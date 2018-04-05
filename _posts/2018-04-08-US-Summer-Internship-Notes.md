---
layout: post
title: 2018北美實習總結
---

美國軟體工程師就業形勢，隨著川普上任以及大量國際學生湧入，實習、找正職的難度不斷飆升。我在2017 Fall來美國後，感受到時局的艱難，花了半年一共面試了18家左右的公司，覺得還是蠻多東西值得分享，因此做了點小數據分析，希望能總結今年的情勢並分享，讓之後來美國找實習的朋友有所幫助。

本篇著重於我會盡量以客觀的角度分析，如有不妥或是錯誤，歡迎提出與討論:)

<!-- more -->
## 目錄
0. <a href="#zero">前言</a>
1. <a href="#one">The very first step: 如何拿到面試</a>
2. <a href="#two">如何面試</a>
4. <a href="#three">總結</a>
<br>  

<a name="zero"></a>
## 前言

<a name="one"></a>
## 一、如何拿到面試
先來談談管道。  
首先要瞭解自身定位，才能對不同管道訂立策略    
1. _**人脈**_ 校友若在美國工作的很多，請盡量找內推，背景不夠好的更要想辦法做connection
2. _**校內競爭力**_ 評估一下履歷profile強度若能比同儕高上一個標準差，就該利用Career Fair以及學校的資源。有個要注意的是很多大公司對於各間學校招聘人數是固定的，比方說今年Microsoft在UCLA就定了要招15個左右的intern（數據由在微軟工作有幫忙校招的朋友提供），你的競爭對手其實不是校外，而是包含undergraduate的同校同學。而program size也會有影響，縱使是Top 1的CMU，一家公司不可能全部都招他們的學生，但CMU畢竟還是牛，我認識台大朋友在CMU的平均拿到五個左右的面試就拿到了offer；類似的大校如USC就有點慘，聽說今年找實習不太理想，個人認為就是因為收的人太多。
3. _**校外競爭力**_ 假設學校名聲與排名夠好，海投一兩百家一定會拿到一些面試機會

接著討論拿到面試的關鍵因素，以及寫履歷的tips。
https://bcf.princeton.edu/master-in-finance/mfin-directory/
我的大學基礎很差，成績更差，但是我用了一些方法讓我履歷看起來很牛

找實習，不論用什麼管道投履歷，時機很重要。

這是我各種管道拿到面試的分布(不包含OA, take home assignment)，左至右按時間排序，深色為拿到offer

> * 內推 5/10  
> Google/Salesforce/LinkedIn\*2/Nutanix  
> * 學校 7/21  
> Microsoft/**textpert** (LA)/**Strategic Global Service** (LA)/Intel/AppFolio (Santa Barbara)/DataHero (LA)/Qualcomm
> * 海投 6/150+  
> **Tencent** (China)/TripAdvisor/MuleSoft/D.E.Shaw/ROW/**PayPal**
> * Recruiter 主動聯繫 1/1  
> SEA (Singapore)

#### Skill Set
CS最多的職缺是general software development engineer，接著是front-end、back-end、mobile，再來是machine learning、data science、research scientist。以intern來說，specific的position還會再更少。

Skill Set Match
    工作經驗
        有大公司實習/工作經驗 > 有實習/工作經驗 > > > 沒經驗
    研究/project經驗

Program reputation

#### 地緣
很多人來美國前選校對於地緣優勢都會有個誤解，覺得要選加州學校，因為離矽谷近。我面試LinkedIn前，被問了這樣的一個問卷調查
> Are you willing and able to relocate to the Bay Area? Are you from a school address that is within 50-mile radius of Linkedin?  

加州很大，所謂的距離近，是可以從學校開車一小時左右到達公司。舉例來說，LA的學校像是UCLA和USC，地緣優勢只能體現在大洛杉磯地區的小新創和少數大公司如Snapchat、Tinder；對於矽谷公司而言，洛杉磯的UCLA跟伊利諾的UIUC相比並沒有太明顯的地理優勢。

#### GPA
請想辦法維持在3.5以上，不少公司會用這個來篩掉成績太爛的candidate，為了學到東西修了一個給分爛workload重的課就本末倒置了，修什麼課沒人care，線上課自學成效也可以很好。個人認為GPA對於海投還蠻重要的，在如果沒有知名大公司實習、頂級名校、足夠Match的經驗下，他是個少數能拿來通過screening的籌碼而且比較好操作，我3.94/4.0的GPA就是策略性修課洗出來的。

以下幾點是我認為幫助我拿到面試機會的主要因素，按重要性排序：
1. 工作經驗: ML intern at KKBOX、DS intern at 遠傳
2. 研究經驗: NLP research at UCLA，騰訊、Global Strategic Service以及小新創textpert都是搞NLP的position
3. 台大: 由於台大在美國業界的人很多，內推幾乎都是請同學或學長姊幫忙
4. LA: 由於矽谷已經趨近飽和，越來越多新創選擇來LA發展
5. 學歷: 大學念CS、美國名校CS碩且高GPA

經驗，尤其是工作經驗重要性今年看下來極明顯。雖然我的實習一不是大公司，二不是在美國，三不是SDE，但是我做的工作內容有實際且可量化的貢獻，跟有些沒實習經驗或是太水的非大公司實習同學相比，拿到了明顯更多的面試。
研究經驗會比project experience有用很多，而且能夠有個明顯的skill set match，

### 內推 (50%)
可以明顯看到內推拿到面試的比例還是遠高於其他方法，主要為:
* 靠人脈(認識)
    * 請朋友
    * 請朋友的朋友 or 同事
    * 跟面試過的同學要公司recruiter的email 
* 靠臉皮(不認識)
    * LinkedIn找校友  
    * 一畝三分地內推版

### 學校資源 (30%)
包含Career Fair、職涯中心(Career Center)、系上的轉發郵件、公司獨立來學校辦的Info Session。每間學校的差異非常大，我在UCLA的Career Fair拿到的面試是零；然而每週的tea time就拿到了Microsoft、AppFolio、Strategic Global Service；轉發的email拿到了Qualcomm、DataHero。

#### Career Fair  
如果自己的背景跟學校的同學相比沒這麼突出，那Career Fair更大的作用是問資訊，比方說自己在front-end experience比較多，就可以問問今年招不招front-end

專注於找到一些會跟你「互動」的公司，比方說我們今年Bloomberg、TripAdvisor、VISA、Laserfiche有當場考coding，這種最好，因為會有較大的機率給通過coding的人面試機會；而大部分公司是會跟你聊聊，說明公司有什麼職缺、在做什麼，然後在你的Resume上記錄，這時候就是跟你學校同儕競爭，一家公司可能收一兩百份簡歷最後只會發十幾個interview；Career Fair上建議不要去排FLAG，因為大多數情況他們會叫你回去網申，你寶貴的一小時排隊就浪費了，像Google就很不客氣的說你們別給我們簡歷了，之後這些都要丟垃圾桶。

大部分學校的Career Fair都很擁擠，像菜市場那樣，每個攤位面前都會排很多人，我們Fall的Career Fair平均一個攤位要排半小時到一小時，端看公司名氣。所以那幾天會很心累
策略：Career Fair的特色在於，有些公司會當場考coding，有些公司會在那一兩天從一兩百份履歷中，選出少數一些人發on campus interview，有些則是會給phone interview。建議一開始就瞄準非FLAG的大公司，因為你會花上一個多小時排隊，最後他們會說請你上網申請......；我們這次有發on campus的有Microsoft、Adobe、Bloomberg、eBay、TripAdvisor、PayPal、

Laserfiche

#### CS Night
UCLA有個晚上邀請了約三十到五十家公司都是CS的缺。

Bloomberg  
一個光頭美國壯哥聊兩句馬上問你會coding嗎，就現場手寫。
Question: 給一個string比方說cccbbaddd，計算各個照字母出現次數並按alphabetical排序，a:1 b:2 c:3 d:3
但Career Fair完不到兩週intern position就full了...

#### CS tea time
我們系上每週三下午會有tea time，偶爾會邀請到公司來給talk以及收履歷。這半年有邀到過Microsoft, AppFolio, Facebook, 

#### Campus Info Session
很多公司會特地到學校租個場地宣傳，各家公司方式都不太一樣，幸運的會遇到願意收履歷、招聘，然後通常有Free Food，肚子餓的話可以單純去蹭飯哈哈。來我們學校的有:

* Twitter: 擺明說不收履歷，浪費大家時間
* VISA: 說明intern program，給了個連結要我們網申
* Amazon A9: 大概給了一個多小時的tech talk，最後有收履歷
* Intel: 他們有一場直接邀請跟同學共進午餐，名額有限得早點報名並且提前到場才有位子。我聽到很多有去吃飯的都有拿到面試。
* Tinder: 雖然沒有招聘，但是跟同學分享面試的技巧，還分開帶大家到小教室做Mock Interview
* Green Hills: 介紹公司、實習，最後有收履歷

### 海投(5%)  
我自己使用最多的是LinkedIn的easy apply，
LinkedIn apply
https://www.intern.supply  


<a name="two"></a>
## 二、面試套路

http://www.1point3acres.com/bbs/thread-105717-1-1.html

<a name="three"></a>
## 三、今年就業形勢

去年Fall時，Amazon宣布了new grad人事凍結這個令人震驚的消息時，一畝三分地板主Warald寫了篇<a href="http://www.1point3acres.com/amazon-stop-sourcing-new-candidate/">今年CS找工作進入了就業寒冬</a>。而intern就我所知，基本上要有身分才能拿到面試（如果有非公民卻在今年拿到面試並錄取的，請糾正我）。有一說法是亞麻為了因應川普對外國人的打壓政策，去年就提前將今年國際生headcount也一併釋出並提前招滿，才會在2016/2017看到一兩輪OA就拿到亞麻、亞麻很水的這種特殊狀況，如果屬實，那不得不佩服亞麻的高瞻遠矚，同時也讓人擔憂國際生接下來的就業處境。

過去幾年只要是CS畢業並且有好好刷題，沒有FLAG也有二三線的科技公司offer。今年不論full time or intern，可以感受到就業市場對國際生滿滿的惡意，很多優秀的同學還是拿不到offer，也有聽到Google intern在找Full time處處碰壁等例子。各公司縮招，運氣成分佔很重，我一個好友面了FB兩輪前端的實習，表現很好且positive feedback，但人事凍結最後就沒下文了；我自己LinkedIn面試big data engineer intern，兩輪interview feedback positive，coding題都給了最優解思路也清晰，其中一輪面試官還特別喜歡我給了bonus題要幫我加分，感覺很穩了，想不到掛在recruiter太晚安排我面試，面完幾天後打來說已提前招滿，很挫敗也很氣憤，連這樣也拒，但也只能摸摸鼻子move on。

http://www.1point3acres.com/about-diversity-hiring/
另一個是蠻多人討論的diversity爭議。我相信diversity的政策在美國一直都有，只是過往人人有一杯羹能分的情況已不復存在，女生性別優勢被放大，同等優秀的情況下，女生會先被考慮。也有少數公司做的蠻過分，像我有一位強者學長有Airbnb intern，他們校區拿到的六人中，只有他一個男生，且其中一個女生還不太會coding...，但也沒辦法，這種比較健康的環境工作。我個人倒是很支持diversity政策的，自己從高中讀男校到大學研究所都是處在病態的性別比環境，未來上班的環境如果又是滿滿的邋塌臭宅男，真的很讓人倒盡胃口。

