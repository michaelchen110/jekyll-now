---
layout: post
title: Learning Global Features for Coreference Resolution
---

_NAACL 2016 | [PDF](http://nlp.seas.harvard.edu/papers/corefmain.pdf)  
Sam Wiseman, Alexander M. Rush, and Stuart M. Shieber_

<!-- more -->

The process of linking together mentions that relates to real world entities is called coreference resolution, which is fundamentally a clustering task. In this post, I will briefly introduce how to learn global features for coreference task using Recurrent Neural Network (RNN). The main contribution in this work is utilizing RNNs to produce feature representations of entity clusters. 

(If you'd like to understand more about coreference, I recommend this clear and in-depth [survey](https://pdfs.semanticscholar.org/c96f/7099e2e8b6d402440700ca5fd2bf247ca81f.pdf)) 

{% include image.html url="/images/2017-11-18/greedy-rnn-prediction.png" description="Figure1: Coreference Resolution" %}

## Motivation

There is compelling evidence that coreference prediction would benefit from modeling global information about entity-clusters. Nevertheless, there exists a trade-off in reality:

* __Global Features Issues.__ While global context is indeed necessary for further improvements in coreference resolution, using a completely local, mention-ranking system can achieve state-of-the-art results. A major reason, as noted by Clark and Manning (2015), is that cluster-level features can be hard to define,  limiting their effectiveness. 

* __Pronoun Problems.__ On the other hand, when resolving pronominal mentions in a purely local way, it generated a substantial percentage of the total errors. Wiseman et al. (2015) show that on the CoNLL 2012 English development set, almost 59% of mention-ranking precision errors and almost 24% of recall errors involve pronominal mentions.

To solve above dilemma, this paper presents an elegant way to learn latent, global representations of entity clusters directly from their mentions using RNN. Such global representations are especially useful for __resolving difficult pronominal mentions__, and can be incorporated into an end-to-end coreference system.  

## Learning Global Features

To learn cluster-level feature representations implicitly, we can identify the state of a (partial) cluster with the hidden state of an RNN that has consumed the sequence of mentions composing the (partial) cluster.

#### RNNs for Cluster Features
We view a cluster _X_ as a sequence of mentions (ordered in linear document order). Then we embed the states of _X_ by running an RNN over the cluster in order:

{% include image.html url="/images/2017-11-18/rnn-states.png" description="" %}

Concretely, this can be implemented by maintaining M RNNs – one for each  cluster – that all share the parameters θ. By doing so, we will effectively run an RNN over each cluster _X_ in the document, and thereby generate a hidden state hj corresponding to each step of each cluster in teh document. We can now dive into core ideas and the model.

#### Full Model
 The original problem can be formalize to an objective function, which aim to maximize the score of both a local mention ranking term _f(x, y)_ as well as a global term _g(x, y, z)_ based on the current clusters:

{% include image.html url="/images/2017-11-18/training.png" description="" %}

Below is local mention ranking where _u_ and _v_ are the parameters of the model, and _ha_ and _hp_ are learned feature embeddings of the local mention context and the pairwise affinity between a mention and an antecedent, respectively:
{% include image.html url="/images/2017-11-18/f.png" description="" %}


We now specify our global scoring function g based on the history of previous decisions. Define _hn_ as the hidden state of cluster m before a decision is made for x – that is, _hn_ is the state of n cluster m’s RNN after it has consumed all mentions in the cluster preceding _xn_. We define g as:
{% include image.html url="/images/2017-11-18/g.png" description="" %}

In traing pass, three metrics were used here, i.e. “false link” (FL), “false new” (FN), and “wrong link” (WL) mistakes (Durrett and Klein, 2013), which correspond to predicting an antecedent when non-anaphoric, ε when anaphoric, and the wrong antecedent, respectively. We typically think of FN as representing recall errors, and FL and WL as representing precision errors. Then the whole system can be learned end-to-end using backpropagation.

## Experiment Result

Here is the main result: 
{% include image.html url="/images/2017-11-18/table1.png" description="Table1: Results on CoNLL 2012 English test set" %}
We see a statistically significant improvement of over 0.8 CoNLL points over the previous state of the art,  and the highest F1 scores to date on all three CoNLL metrics. 

Furthermore, we find that the RNN imporves performance overall with the most dramatic improvements on non-anaphoric pronouns, though errors are also decreased significantly for non-anaphoric nominal and proper mentions that follow at least one mention with the same head:
{% include image.html url="/images/2017-11-18/table2.png" description="Table2: Number of errors on non-anaphoric (top) and anaphoric (bottom) mentions" %}
Importantly, the RNN performance is significantly better than that of the Avg baseline. This suggests that modeling the sequence of mentions in a cluster is advantageous.

#### Comparison & Analysis
The impact of the g term in the RNN scoring function on the two error categories that improve most under the RNN model (as shown in Table 2), namely, pronominal WL errors and pronominal FL errors. In order to explain the difference, this paper provided two example regarding __pronoun__:

|
:-------: | :-------:
![config.yml]({{ site.baseurl }}/images/2017-11-18/his.png)|![config.yml]({{ site.baseurl }}/images/2017-11-18/its.png)
 Figure2: Ambiguous Pronoun *`his`* | Figure3: Ambiguous Pronoun *`It's`*

In Figure2, baseline MR incorrectly predicts *__his__* to corefer with the closest gender consistent antecedent *__Justin__*, thus, making a WL error; on the other hand, greedy RNN correctly predicts *__his__* to corefer with *__Mr.Kaye__* in the previous sentence. We see that when the initial *__Justin__* mentions are added to X(1) the g-score is relatively high. However, after *__The company__* is correctly predicted to corefer with *__Justin__*, the score of X(1) drops, since companies are generally not coreferent with pronouns like *__his__*.

In Figure3, MR predicts *__It's__* to corefer with a previous *__it__*, making a FL error; while the Greedy RNN model does not. *__It's__* is being used
pleonastically. We observe that both of the potential antecedent *__S-Bahn__* and initial pleonastic use of *__It's__* have large gradient, implying that easier, earlier predictions of pleonasm can inform subsequent predictions.

## Conclusion
The authors presented a simple framework to integrate global information in coreference resolution, while avoiding manually defining global features. This novel architecture is especially useful when consider implementing an end-to-end coreference system, which is a building block in future works.  

<!--{% include image.html url="/images/2017-11-18/t-sne.png" description="Figure2: Entity Representations" %}-->
