---
layout: post
title: Character Identification in Multiparty Dialogue with Neural Coreference Resolution
---

[Video](https://www.youtube.com/watch?v=2OkvUVwokHM) | 
[PDF](https://github.com/michaelchen110/e2e-coref/blob/master/report/acl2016.pdf) | 
[Github](https://github.com/michaelchen110/e2e-coref)

<!-- more -->

## Introduction
Our main goal is to accomplish a shared task in SemEval 2018 - Task 4: Character Identification on Multiparty Dialogues. This tasks requires us to build a system which can identify different mentions in multiparty dialogues as corresponding characters in the show. To illustrate with the following picture, the mention “dad” is not one of the speakers.Instead, it is obviously referred to the specific person, Jack, who may appear during some other conservations. This task is rather challenging, for cross-document entity resolution is imperative for identifying such mentions as real characters.

{% include image.html url="/images/2017-12-11/semeval2018task4.jpg" description="Example of character recognition" %}

Literally, the character identification problem is tackled as a coreference resolution task with a further step on entity linking.In terms of this task, the baseline model generates mentions from a coreference system, and then each coreference chain is linked to a specific character identity. Both parts are implemented with agglomerative convolutional neural network in previous system (Chen et al., 2017; Chen and Choi, 2016). Alternatively, we intend to use Bidirectional-LSTM with attention mechanism to address the same problem, which proves to have a satisfying performance in many NLP tasks. In our project, we apply the end-to-end neural coreference resolution model introduced by Lee and He, etc. (Lee et al., 2017). After obtaining the predicted clusters of mentions by the end-to-end coreference system, we choose the same algorithm of entity-linking as the one Chen proposed in his paper.

## Related Works
### Coreference Resolution
Machine learning methods have a long history in coreference resolution. However, the learning problem is challenging and, until very recently, hand-engineered systems built on top of automatically produced parse trees (Raghunathan et al., 2010) outperformed all learning approaches. Durrett and Klein (2013) showed that highly lexical learning approaches reverse this trend, and more recent neural models (Wiseman et al., 2016; Clark and Manning, 2016b,a) have achieved significant performance gains. However, all of these models still use parsers for head features and include highly engineered mention proposal algorithms.Such pipelined systems suffer from two major drawbacks: (1) parsing mistakes can introduce cascading errors and (2) many of the hand-engineered rules do not generalize to new languages or domains.

The end-to-end coreference resolution model we used in this task significantly outperforms all previous work without using a syntactic parser or hand-engineered mention detector.

### Entity Linking
Entity linking has traditionally relied heavily on knowledge databases, most notably, Wikipedia, for entities (Mihalcea and Csomai, 2007b; Ratinov et al., 2011b; Gattani et al., 2013; Francis-Landau et al., 2016).3 Although we do not make use of knowledge bases, our task is closely aligned to entity linking. Recent advances in entity linking are
also applicable to our task since we see Francis-Landau et al. (2016) use convolutional nets to capture semantic similarity between a mention and an entity by comparing context of the mention with the description of the entity. This work validates our
usage of deep learning for character identification.

Dialogue tracking has been an expanding task as shown by the Dialogue State Tracking Challenges hosted by Microsoft (Kim et al., 2015). That an ongoing conversation can be dynamically tracked (Henderson et al., 2013) is exciting and applicable to our task because the state of a conversation may yield significant hints for entity linking and coreference resolution. Speaker identification, a task similar to character identification, has already shown some success with partial dialogue tracking by dynamically identifying speakers at each turn in a dialogue using conditional random field models.

## End-to-End Coreference Resolution
Recent coreference models usually rely on syntactic parsers. However, the end-to-end coreference resolution directly consider all the spans up to a maximum length in the document as potential mentions,  compute the probability of possible ancestors (previous span) for each span, and directly optimizes the marginal likelihood of antecedent spans from gold coreference clusters.

Since the number of potential mentions is very large, it is impractical to score all span pairs. So this model uses unary mention scores to prune the space of pairs of spans(spans and antecedents), which significantly reduce the pairwise computations.
### Model
{% include image.html url="/images/2017-12-11/model1.jpg" description="Coreference Resolution: Step 1" %}
First step: computes embedding representations of spans for scoring potential entity mentions.
A  bidirectional LSTM (Hochreiter and Schmidhuber, 1997) to encode the lexical information of both the inside and outside of each span. The model also includes an head-finding attention mechanism over words in each span to model head words.
Low-scoring spans are pruned, so that only a manageable number of spans is considered for coreference decisions.

{% include image.html url="/images/2017-12-11/model2.jpg" description="Coreference Resolution: Step 2" %}
Second step: compute antecedent scores from pairs of span representations. And then sum the mention scores of both spans and their pairwise antecedent score as the final coreference score of this pair of spans.
The antecedent scoring function includes explicit element-wise similarity of each span pair and a learned 20-dimensional feature vector which encoding all features like speaker genre, span distance, mention width.

### Learning
We optimize the marginal log-likelihood of all correct antecedents implied by the gold clustering:
{% include image.html url="/images/2017-12-11/learning.jpg" description="MLE Learning" %}
where GOLD(i) is the set of spans in the gold cluster containing span i. If span i does not belong to a gold cluster or all gold antecedents have been pruned, GOLD(i) = {}.

### Ablations
To show whether each component in our model is actually important, we ablate various parts of the architecture and report the average F1 on these experiments. We conducted one complete experiment and two ablation experiments, no heads and no features. The result of these three experiments is shown in Chapter 6.

## Entity Linking
Once the coreference resolution system is built and trained, we can predict co-references represented by clusters for each scene document. The next step should be making predictions from clusters to TV show character id. We model this process as an entity linking task. This section describes our entity linking model that takes the mention embeddings and the mention-pair embeddings generated ACNN and classifies each mention to one of the character labels.

{% include image.html url="/images/2017-12-11/model3.jpg" description="" %}
We prepare three embeddings generated by mentions which are predicted by precious co-reference system. The first embedding is mention embedding; the second is embedding of the cluster including the mention; the third is generated by mention-pair embedding, which pairs the mention with reaming mention in the same cluster. Here are the formal formula:
{% include image.html url="/images/2017-12-11/formula1.jpg" description="" %}
In order to fix the input tensor size of both cluster embedding and mention-pair embedding, we perform avg-pooling and max-pooling for both embeddings. Then each of pooling layers is passed to a convolutional layer. Finally, we concat the mention embedding, cluster CNN embedding and mention-pair CNN embedding. 
{% include image.html url="/images/2017-12-11/formula2.jpg" description="" %}
After concatenation, we feed them into a feed-forward neural network with two hidden layers. Final output is a softmax with the idmention of entity id number in Friends TV show.

## Dataset and Evaluation Metrics
### Data Description
The data comes from the scripts of the first two seasons of TV show Friends, which are already annotated for this task. Specifically, each season consists of episodes, and each episode is comprised of scenes. Furthermore, each scene is segmented into sentences.All datasets follow the CoNLL 2012 Shared Task data format. Each sentence is delimited by a new line and each column indicates the following information regarding the word or the punctuation.
* Document ID: /(name of the show)-(season ID)(episode ID) (e.g., /friends-s01e01).
* Scene ID: the ID of the scene within the episode.
* Token ID: the ID of the token within the sentence.
* Word form: the tokenized word.
* Part-of-speech tag: the part-of-speech tag of the word (auto generated).
* Constituency tag: the Penn Treebank style constituency tag (auto generated).
* Lemma: the lemma of the word (auto generated).
* Frameset ID: not provided (always '\_').
* Word sense: not provided (always '\_').
* Speaker: the speaker of this sentence.
* Named entity tag: the named entity tag of the word (auto generated).
* Entity ID: the entity ID of the mention, that is consistent across all documents

{% include image.html url="/images/2017-12-11/data.jpg" description="CoNLL data format" %}

### Data Preprocessing
Our training data has 374 documents, which contains totally 13280 gold mentions that have gold entity label. Firstly, we need to get gold clusters and generate three embeddings, i.e. mention, cluster and mention pair embeddings. Since all gold clusters are labeled with entity ids, we can flat clusters to mentions while computing three embeddings. We can easily get mention embeddings from the pretrained coref model.

Considering the amount of total data is not so sufficient, we simply split them into two datasets for different purposes, training and evaluation sets. The exact ratio of our training set to our evaluation set is 4:1. The evaluation set contains seventy-four scenes in Friends.

### Coreference Evaluation Metrics
The coreference results are evaluated with three metrics apropos coreference resolution: MUC, B3,and CEAFe. The precision, recall and F1 score of each metric approach are calculate separately and then the averages of them are obtained, which are utilized to compare against each other.
#### MUC
MUC(Vilain et al.,1995) concerns the number of pairwise links needed to be inserted or removed to map system responses to gold keys.The number of links shared by  system and gold are calculated. In addition,minimum numbers of links needed to describe coreference chains of the system and gold are computed as well.

#### B Cube
Rather than evaluating coreference chains merely on their links,B3(Bagga and Baldwin,1998) metric computes precision and recall on a mention level.System performance is evaluated by the average of all mentions scores.

#### CEAF_e
CEAFe  (Luo,2005) metric further clarifies the downside of B3, in which entities can be used more than once during evaluation. Consequently, both multiple coreference chains of the same entity and chains with mentions of multiple entities are not penalized.To mitigate the aforementioned problem, CEAFe  evaluates exclusively on the best one-to-one mapping between the system’s and gold’s entities. 

## Results and Analysis
We conducted one complete experiment and two ablation experiments, no heads and no features. The result is shown in Table 1:
{% include image.html url="/images/2017-12-11/result.jpg" description="Table 1" %}
It can be found that no head experiment has higher score than normal experiment. The reason is in this project, most mentions in the dataset are just one word, which means mention start, mention end and mention head are the same one.

## Conclusion and Future Work
In this work, we imply an end-to-end character identification system, combining neural coreference system with an agglomerative convolutional neural network entity linking model. The results should be improved in the future if we can gather GPU resources. Inspired by (Clark and Manning, 2016), the next step will be designing loss function proposed in their work and boost the reliability of our system using reinforcement learning. 

I am still working on this. So if you have any idea, please don't hesitate to contact me!
