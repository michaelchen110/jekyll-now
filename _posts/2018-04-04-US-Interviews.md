---
layout: post
title: 2018北美實習面經
---

這邊整理了我在找2018 summer intern面試的17家公司，接近30輪interviews，還有5家OA/Take home assignment。先分類、再按照面試時間排序。

<!-- more -->

1. <a href="#big">大公司</a>
    * 10.25 <a href="#microsoft">Microsoft</a> 
    * 12.13 <a href="#google">Google</a> 
    * 12.20 <a href="#salesforce">Salesforce</a>
    * 01.25 <a href="#linkedin">LinkedIn</a>
    * 02.14 <a href="#intel">Intel</a>
    * 02.16 <a href="#paypal">PayPal</a> (offer)
2. <a href="#startup">中小型、新創</a>
    * 11.07 <a href="#textpert">Textpert</a> (offer)
    * 12.14 <a href="#appfolio">AppFolio</a>
    * 01.10 <a href="#tripadvisor">TripAdvisor</a>
    * 01.27 <a href="#mulesoft">Mulesoft</a>
    * 02.16 <a href="#datahero">DataHero</a>
    * 03.26 <a href="#nutanix">Nutanix</a>
3. <a href="#finance">金融</a>
    * 11.02 <a href="#sga">Strategic Global Service</a> (offer)
    * 01.17 <a href="#deshaw">D.E.Shaw</a>
    * 02.15 <a href="#row">ROW Asset Management</a>
4. <a href="#oversea">海外</a>   
    * 11.06 <a href="#tencent">Tencent 中國騰訊</a> (offer)
    * 12.28 <a href="#sea">SEA</a>
5. <a href="#oa">OA/Take Home Assignment</a>   
    * <a href="#twitter">Twitter</a>
    * <a href="#ebay">eBay</a>
    * <a href="#citadel">Citadel</a>
    * <a href="#squarespace">Squarespace</a>
    * <a href="#adobe">Adobe</a>

<br>

- - - 

<a name="big"></a>
## 一、大公司 (10,000+ employees)

<a name="microsoft"></a>
### **Microsoft**
#### _CS tea time | Software Development Engineer Intern_
這是我來美國後第一個面試，花了一週把MS tag的高頻都做了，leetcode從6x題刷上100題。微軟簡歷篩的很兇，算是比較難拿到面試的，但由於微軟注重綜合素質，準備時要對behavior questions (BH)下功夫。我犯了個錯誤，在面試前全力衝刺leetcode，沒準備BH，結果就面掛了。

**on campus (UCLA career center)**   
_30 mins_ ，美國男 manager  
互相自我介紹，接著問一道super easy題，花了五分鐘在紙上寫完。
> Q1. Odd Number   
> Input: String  
> Output: number of odd words  
>
>     e.g. Input: Hi! How are you?   
>          Output: 3 (How are you)
>
> Q1 Follow Up.  
> How would you design test case?
>     
>     * null string
>     * special characters
>     * input string with more than 2^32 odd words

接下來二十五分鐘全在問Behavior Questions
> * What's your best team work experience?
> * What's your worst team work experience?
> * How would you avoid this bad cooperation situation next time? 
> * Tell me your favorite project.
> * Tell me the most difficult situation in your prior working experience.
> * There many teams in Microsoft, which team do you want to join the most?

其他人被問到的LC題
> * Tree Level Order Traversal
> * Least Common Ancester

如果有通過，就會直接onsite 4 round。
    
### **Google**
#### _內推 | Research Intern_

Google請人內推完以後，會收到一封確認信然後選擇三個要申請的position。我那時候內推完沒有收到信，以為這樣就沒問題了，後來過了SDE intern application deadline我才發現沒有內推到，請朋友再內推一次時只剩下research intern了，只好硬著頭皮上。

面試Research intern前，HR會給一個問卷讓你提供你的研究方向，我當時是選NLP，結果他幫我schedule了一個CV方向的人面我，於是我趕緊寄信讓他更正。 

**1st phone interview (research)**  
_45 mins_ ，中國大哥  
簡單介紹他的team在做NLP後，我也自介，接著就開始問我在UCLA NLP lab做的研究。我先介紹multi dialgue using neural coreference resolution的task，接著講model。對方問說問何這邊要用attention mechanism？我就解釋了下；然後又問對於代名詞的部份，要怎麼有效做coref；

**2nd phone interview (coding)**   
_45 mins_ ，印度小哥  
在第一通電面完後緊接著第二輪。一開始三哥電話還打不通，我才意識到宿舍的訊號太爛。接通後給了Google Doc，
問了一道leetcode原題

    Search min in a rotated sorted array

比較值得一提的是中間的溝通。由於剛來美國，聽印度腔英文真的不適應，加上宿舍收訊巨爛，對方講了很多都沒能聽清楚，因此他很多不用講的，打在Google doc上。當時演戲技能太差又緊張，一開始馬上就講正解用binary search，他就說，我看不出來這哪裡能用binary search，然後就說你要不先用一個簡單的方法吧。我就說O(N)從頭開始找，然後再優化。接著講bianry search做法，簡單解釋一下算法，就開始寫代碼。寫一寫他問為什麼要這樣分if else，我就說就是我前面解釋的那個，然後他說我沒有講，我就很無言，然後給他看上面我打字解釋過的部份再講一次，接著就把它寫完了。不過有syntax error，前幾天寫太多tensorflow，結果用Java不小心沒加分號......被他說：「I think you misuse the other language」。最後說他很surprise我能用這個解法解出來。

誠懇的寫了Thank you letter，一週後HR電話打來拒，而且不給feedback。

### **Salesforce**
#### _內推 | Softwar Engineer Intern_

HR幫我match了search team，並說明兩輪都是1hr technical/behavioral phone interview going over basic CS concepts, algorithms, data structures, and coding

**1st phone interview**   
_1 hour_ 美國姊姊 Data Scientist  
全部都在聊我的background。focus在intern experience，也有聊一點research。解釋了我在KKBOX做的deep learning model，如何做personalized recommendation，如何用CNN對audio抽取high level musical feature；以及怎麼把所有東西串成一個deep learning pipeline。最後問了三個問題，過程互動良好，面完給了下一輪。

**2nd phone interview (collabedit)**   
_1 hour_ 美國小哥 Senior SDE  
簡單自介後不囉嗦上題
    
> Q1: Average of a stream of numbers  

給了一個O(1)解法

> Q2: Variance of a stream of numbers

也是要O(1)。寫到一半collabedit網站掛掉無法協同編輯code，只好把我寫好的code email給他......

    double suqare = 0;
    double linear = 0;
    int count = 0;
    int sum = 0;

    public double variance(int nums) {
        int mean = 0;
        
        count++;
        linear += nums;
        square += Math.pow(nums, 2);
        mean = linear / count;
        
        sum += Math.pow(square, 2) - 2 * linear * mean + Math.pow(mean, 2);
        return sum / count;
    }

其實前一晚太緊張失眠，當下狀況也不好瞬間忘記variance的公式，讓他提醒了......，結果後來就跪了。

### **LinkedIn**
#### _內推 | Big Data Engineer Intern_
Major components of our assessment include:
- Application of algorithm and Computer Science fundamentals
- Explanation and implementation of the solution in code without any of the aids engineers typically have access to (e.g. IDE, online docs)
- Any DBMS knowledge is a positive and questions will be asked on the basics and architecture of DBMS.

**1st phone interview (collabedit)**  
_1 hour_ 中國小哥 Senior SDE  

> Leetcode 200. Number of Islands

    //Time O(grid)

    public int islands(int[][] grid) {
        if (grid == null | grid.length == 0 || grid[0].length == 0) return 0;
        int count = 0;
        boolean[][] used = new boolean[gird.length][gird[0].length];
        Arrays.fills(used, false);
        
        for (int i = 0; i < grid.length; i++) {
            for (int j = 0; j < grid[0].length; j++) {
                // encounter each newly found island 
                if (grid[i][j] == 1 && !used[i][j]) {
                    count++;
                    dfs(grid, used, i, j);
                }
            }
        }
        return count;
    }

    private void dfs(int[][] grid, boolean[][] used, int i, int j) {
        // check boarder and check if [i, j] pair is used and valid(1)
        if (i < 0 || i >= grid.length || j < 0 || j >= grid[0].length 
           || grid[i][j] == 0 || used[i][j]) return;
        used[i][j] = true;
        // 4 dfs up/down/right/left
        dfs(grid, used, i, j - 1);
        dfs(grid, used, i, j + 1);
        dfs(grid, used, i + 1, j);
        dfs(grid, used, i - 1, j);
    }

> Leetcode 236. Lowest Common Ancestor of a Binary Search Tree    

    // p , q may not even exist in tree
    public TreeNode LCA(TreeNode root, int p, int q) {
        if (root == null) return root;
        
        while ((root.val - p) * (root.val - q) > 0) {
            if (root == null) return root;
            root = p > root.val ? root.right : root.left;
        }
        
        //still need 2 BST 
        
        return root;
    }

    // visualization

                1
            root.val 
        /             \
                        20 
                         /
                        3                                
                         \           
                          LCA(10)
                            /         \
                                        15
                         5 p(null)            \ 
                                           q(17)      
              

被問說如果p, q不在tree裡面怎麼辦，我就說要先做兩個binary search。寫完解釋完時間也差不多了。問了幾個問題像是你們組都用什麼工具、workflow等等。


**2nd phone interview (collabedit)**  
_1 hour_ 美國大哥 Senior Data Engineer  
自介的時候特別強調了在遠傳data science intern做database optimization，improve了一個重要query 300X的效能，從一星期reduce到半小時，讓老人家很amazing。不過這邊有個插曲。大約講了六分鐘後電話就斷線了，重打接通後繼續，花了些時間解釋我怎麼做優化的。接著他就說我來看看要考你什麼題（能感覺出他手上有一疊題庫，隨機抽考)

> Q1: isNumber

    /*
     * Returns true if the input string is a number and false otherwise
     */

    //+1
    //-1
    //1.0
    //32
    //.2

    import java.util.*;

    public class TEST{
        public static void main(String[] args) {
            System.out.println(isNumber("1.0"));
        }
        public static boolean isNumber(String toTest)
        {
            // implementation here
            boolean sign = false;
            for (int i = 0; i < toTest.length(); i++) {
                if (i == 0 && toTest.charAt(i) == '+' || toTest.charAt(i) == '-') continue;
                if (toTest.charAt(i) == '.') {
                    if (sign) return false;
                    else sign = true;
                }
                else if (toTest.charAt(i) >= '0' && toTest.charAt(i) <= '9') continue;
                else return false;
            }
            return true;
        }
    }

> Q2: How often would you load streaming data in your previous internship?

解釋了我在遠傳怎麼處理海量streaming data，多久update一次

> Q3: 各種SQL 非常基礎的知識，像是group by在幹嘛、要注意什麼等等

過程溝通的很愉快也很順暢，到這邊面試官突然說，我非常喜歡你，想給你一個bonus題幫你加分
> Q4: Bonus: Given that you have all data in grocery stores, what kind of data will you collect, and how will you design your schema in order to analyze selling performance?

比方說商品擺放位置、商店location、每個transaction同時出現的items.....；然後還跟他說data mining的一些概念，舉了例子比方說可樂打折但是薯片漲價，來提高selling performance

最後他說他非常喜歡我，希望能加入LinkedIn，還說會給我strongly recommend to recruiter。面試完相當激動，覺得努力很久終於有收穫了，唯一一個可能就是提前招滿，但是HR跟我schedule的時候說這個position才剛開始，感覺很穩了。

過幾天後HR打來說你的feedback positive但招滿了。。。。。。打擊非常大，畢竟是我表現最好的的兩個面試，想不到這樣還能被拒。

#### _內推 | Data Science, Analytic Intern_ 
The interviewer may ask you problem solving questions with a LinkedIn business case study. We’re looking to see how you might approach a real-world situation that requires a structured approach and you will be measured on framework, assumptions, and communication in solving these problems. Please go into details on the analytical approach and steps that lead to the conclusions. The interviewer can also go in depth and ask questions on applied statistics/machine learning/probability theory to business problems. We’re looking to understand how you reason with mathematical concepts and inferences.  

**HR Screening**  
_20 mins_   
說data science/data mining intern只剩一個缺，問我要不要面試data science/analytics缺比較多，我秒說好。然後問了一個很簡單的SQL題，類似給一個table with two columns, one is state name and the other is city name，select the top 5 state contain most cities in descending order。直接用講的。 

**1st video interview (collabedit, BlueJeans)**  
_45 mins_ 美國姊姊 Data Scientist  
不囉嗦沒自介，直接到collabedit上開始做題

> Q1: You have 2 tables t1 and t2, each with a single column and the values shown. Write the select statement that performs a left outer join on col1, and show the results.
> 
> INPUT DATA:  
>
>     table t1  
>      col1   col2  
>         1      A  
>         1      A  
>         1      B  
>         2      A  
>         4      C  
>      
>     table t2  
>      col1  col2  
>         1     A  
>         3     B  
>         4     A  
>         4     C    

    -- Solution
    SELECT *
    FROM t1
    LEFT JOIN t2
    ON t1.col1 = t2.col1;
    
    --  col1   t1.col2    t2.col2
    --     1      A         A
    --     1      A         A
    --     1      B         A
    --     2      A         NULL
    --     4      C         A
    --     4      C         C

> Q2: You have a table of views of articles like this:
>  
>     article_views
>     
>     view_date   viewer_id   article_id  author_id    
>     2017-08-01      123         456         789    
>     2017-08-02      432         543         654  
>     2017-08-01      789         456         789  
>     2017-08-03      567         780         432  
>     2017-08-04      789         111         789  
>     2017-08-04      789         111         789  
>
> For each article view, we have the date, the member id of the viewer, the article id of the article they viewed, and the member id of the author who wrote the article.   

> Q2-1. How many article authors have never viewed their own article? 
> 654, 432

    SELECT DISTINCT author_id
    FROM article_views
    WHERE author_id NOT IN (
        SELECT author_id
        FROM article_views
        WHERE viewer_id = author_id
    );

> Q2-2. If there are some duplication? 

    SELECT count(A.id) num_author
    FROM (
        SELECT author_id id, COUNT(DISTINCT article_id) num
        FROM article_views
        GROUP BY author_id
    ) A,
    (
        SELECT author_id id, COUNT(DISTINCT article_id) num
        FROM article_views
        WHERE viewer_id = author_id
        GROUP BY author_id
    ) B
    WHERE A.id = B.id and A.num != B.num;

> Q2-3. Can you solve it using programming language other than SQL?

    public int authors(int[] viewer_id, int[] article_id, int[] author_id) {
        //key: article_id, author_id
        int count = 0;
        Map<Integer[], Boolean> map = new HashMap<>();
        for (int i = 0; i < viewer_id.length; i++) {
            int[] key = {article_id[i], author_id[i]};
            if (map.containsKey(key) && map.get(key)) continue;
            if (viewer_id[i] == author_id[i]) map.put(key, true); 
            else map.put(key, false);
        }
        
        //count the key with true value
        for (int[] key: map.keySet()) {
            if (map.get(key)) count++;
        }
        return count;
    }

**2nd video interview (collabedit, BlueJeans)**  
_45 mins_ 中國小哥 Data Scientist  
> Focus on A/B testing

* There is a dramatic drop of user usage on our website last two weeks. To see what was happening, how would you test?   
* How would you do segamentation?
* Why did you choose age, location, vocation to segament?
* How to sample your data?
* If the p-value is > 0.05, could we conclude that this experiment fail? And what would you do in the next step? 

> 還有基本的統計

* explain type I/type II error
* explain alpha value 
* explain p-value to a person without techical background

A/B testing完全沒學過、統計很多也忘光光，就直接跪了。

### **Intel**
#### _Info Session_  
Intel比較特別，幫軍方做chips，所以對於身分要求很高，查很嚴，只有很少數的人能拿到面試。我在Info session後與裡面的人聊聊，首先就先被問是不是公民，然後說Intel的IT department只收公民，其他的department就沒這個要求。然後跟一個中國大哥聊聊，說自己本來想讀PhD但後來放棄，就說我可以跟你聊聊，要不約個明天吧？蠻妙的竟然是這個原因拿到on campus。  

**on campus (UCLA Career Center)**   
_1 hour_ 中國大哥  
沒有任何的coding，或是技術問題，一小時都是聊天。聊一下我的興趣、做的研究、為什麼想做研究，然後大哥解釋了他們想招的人，是audio signal processing engineer，但是想要用deep learning技術來做，聊了一下產品，還有哪些可能跟我可以做的項目。最後他講他當時讀博到一半quit的故事，鼓勵我如果可以的話，考慮一下讀博哈哈。然後說他會把我推薦給組內還有其他組看有沒有機會match。

然後就沒下文了。

### **PayPal**
#### _海投 | Cloud Engineer Intern_
**1st phone interview**  
_1 hour_ 印度女

> Q1: 如何做Outlier Detection  

首先點出unbalance data問題，然後提出可以用semi-supervised的方法；然後再提出能用density-based clustering像是DBSCAN，並解釋了一下算法。

> Q2: num of distinct words in a document

    public int numdistinct(string[] file) {
        set<string> set = new hashset<>();
        for (string word : file) {
            if (!set.contains(word)) set.add(word);
        }
        return set.size();
    }

> Q3: Implement Bubble Sort 


**2nd video interview (skype)**  
_1 hour_ 印度男
> Q1: Reverse the string

    // in-place
    public String reverse(String input) {
        int len = input.length() - 1;
        int start = 0, end = len;

        StringBuilder sb = new StringBuilder(input);
        for (int i = 0; i < (len + 1) / 2; i++) {
            // swap
            char tmp = sb.charAt(i);
            sb.setCharAt(i, sb.charAt(len - i));
            sb.setCharAt(len - i, tmp);
        }
        return sb.toString();
    }

> Q2: Find top 5 most popular cities.
> 
>     Input:
>     List of favorite cities for users
>     John ->  London, New York, Sydney
>     Mark -> London, Paris, San Francisco
>     Suren -> Paris, Los Angeles, Cicago, Miami

    public List<String> popularCities(List<List<String>> input) {
        Map<String, Integer> map = new HashMap<>();
        Map<Integer, List<String>> sortMap = new TreeMap<>();
        List<String> res = new LinkedList<>();
        int count = 0;

        for (List<String> user : input) {
            for (String city : user) {
                int c = map.getOrDefault(city, 0) + 1;
                map.put(city, c);
            }
        }
        // map
        // London: 2
        // Paris: 2
        // Los Angeles: 1
        // .....

        // London: 2, Paris: 2 duplicate
        for (String k : map.keySet()) {
            List<String> l = sortMap.getOrDefault(map.get(k), new LinkedList<>());
            l.add(k);
            sortMap.put(l);
        }
        // sortMap
        // 2: [London, Paris]
        // 1: [Los Angeles, ...]

        for (Integer c : sortMap.keySet()) {
            for (String city : sortMap.get(c)) {
                if (count == 5) return res;
                res.add(city);
                count++;
            }
        }
        // res
        return res;
    }

**3rd video interview (skype)**  
_1 hour_ 印度男  
接著上一輪繼續面  
> Q1: Leetcode 原題 Best Time to Buy and Sell Stock

遇到插曲，collabedit網站掛掉寫不了code，我就在skype上面打一行說明一行，而且還沒有縮排，但還是有解釋清楚。

> Q2: 各種Java觀念
* What's Polynorphism?
* Why cannot use multiple inheritence? 
* Experience in Tomcat web service?
* 還有一些忘了

HR動作很快，隔天就給了口頭offer。

- - - 
<a name="startup"></a>
## 二、中小型、新創 (\< 5000 employees)

<a name="textpert"></a>
### **Textpert** (\<10 employees)
#### _LA startup fair | NLP intern_
有天學校辦了一個LA startup fair，來了十來家小新創公司，雖然不多但能投的都投了一遍。這家是做NLP的，剛好聊的時候才剛弄玩NLP project，就聊的比較愉快，隔幾天收到面試邀請，就在Anderson的Incubator面試。

**On Campus (Anderson Incubator)**  
**1st behavior questions**  
_45 mins_ 美國CEO小哥  
雙方自我介紹了一下，接著全問行為問題，還有腦筋急轉彎
> Behaviour Questions:
* 你最大的成就是什麼
* 你過去最後悔的事情是什麼
* 你最大的恐懼是什麼
* 回到五年前，你會跟自己說什麼，只有十秒鐘
* 五年後的你回來，會跟自己說什麼，只有十秒鐘
* 想像我在跟其他面試官討論要不要給你這個offer，現在有十秒鐘你會變成我，你會怎麼講？

> Brain Teaser: (1 min/each)
* 一個5L、3L水杯，怎樣在5L燒杯湊成4L水
* 三個燈泡只能看一次，三個開關隨你試，怎樣看一次就知道哪個開關是哪個燈泡
* 一個死亡門、一個自由門、一個誠實人、一個騙子，怎樣只問一個人一句問題，就知道你要走哪個門？ 

**2nd technical**  
_30 mins_ 美國工程師小哥 

> 
* 電話號碼permutation (228 → CBT, CAT, ABU…)
* 如果permutation的字要在字典，要怎麼辦？trie tree
* 現在一個人打字打到一半，I like to (228) ，如果要用deep learning來找出最有可能出現的字來推薦，怎做

**3rd technical**
_30 mins_ 美國工程師小哥 

>    
* 講一下實習項目
* 如果我們有個database，裡面有很多的questions，有一個人問了一個question，要怎麼樣從我們DB找出最相關的那個句子？
    - 需要哪些training data? Tf-Idf
    - 這樣有什麼問題？兩個相似的句子不同長度會變一樣value所以需要RNN

<a name="appfolio"></a>
### **AppFolio** (700 employees)
#### _CS tea time | Software Development Engineer Intern_
**Video Interview (GoToMeeting)**  
_45 mins_ 美國小哥
前面花了比較多時間自介，小哥講了AppFolio在做的，並說雖然實習寫Ruby，但是會給training。接著做題，比較特別，給了一個pseudo code，問會print出什麼，把結果畫在紙上，是個三角形，並對著攝像頭給他看。

<a name="tripadvisor"></a>
### **TripAdvisor** (4700 employees)
#### _海投 | Data Science Intern_
**HR Screening**   
_20 mins_  
自介，然後問behavior questions
* Talk one of your proudest project
* What's TripAdvisor's product?  

家裡訊號太差，講到一半電話斷線了連續六分鐘打不通，過幾天直接收拒信

<a name="mulesoft"></a>
### **Mulesoft** (1400 employees)
#### _海投 | Software Development Engineer Intern_
MuleSoft是一家在SFO的API公司

**HR Screening**  
_30 mins_ 美國大姊  
體驗很差，問基本資料的時候，語速很快像在趕火車，態度也很漫不經心，不太尊重面試者。

**Video Interview (Karat)**  
_45 mins_ 美國大姊  
他們家第一輪面試都會先透過Karat這個招聘平台，由這個平台的員工負責面試並把結果回報，MuleSoft之後就依據回報決定是否給下一輪。

先花了十五分鐘講prior internship experience

> Problem 1: Write a function that takes this input as a parameter and returns a data structure containing the number of hits that were recorded on each domain AND each domain under it. For example, an impression on "sports.yahoo.com" counts for "sports.yahoo.com", "yahoo.com", and "com". (Subdomains are added to the left of their parent domain. So "sports" and "sports.yahoo" are not valid domains.)
>
>       Expected output (in any order):
>       1320    com
>        900    google.com
>        410    yahoo.com
>         60    mail.yahoo.com
>         10    mobile.sports.yahoo.com
>         50    sports.yahoo.com
>         10    stackoverflow.com
>          3    org
>          3    wikipedia.org
>          2    en.wikipedia.org
>          1    es.wikipedia.org
>
>       String[] counts = {
>           "900,google.com",
>           "60,mail.yahoo.com",
>           "10,mobile.sports.yahoo.com",
>           "40,sports.yahoo.com",
>           "300,yahoo.com",
>           "10,stackoverflow.com",
>           "2,en.wikipedia.org",
>           "1,es.wikipedia.org" };


    private static List<String> url(List<String> u1, List<String> u2) {
      List<String> local = new LinkedList<>();
      List<String> global = new LinkedList<>();
      
      int p1 = 0, p2 = 0;
      while (p1 < u1.size()) {
        while (p1 < u1.size() && p2 < u2.size()) {
          String str1 = u1.get(p1);
          String str2 = u2.get(p2);
          if (str1.equals(str2)) {
            local.add(str1);
            if (local.size() > global.size()){
              global = new LinkedList<>(local);
            }
            p1++;
          }
          else {
            local = new LinkedList<>();
          }
          p2++;
        }
        p2 = 0;
        p1++;
      }
      return global;
    }

> Problem 2: We have some clickstream data that we gathered on our client's website. Using cookies, we collected snippets of users' anonymized URL histories while they browsed the site. The histories are in chronological order and no URL was visited more than once per person.  
>  
> Write a function that takes two user’s browsing histories as input and returns the longest contiguous sequence of URLs that appears in both.
>   
>       Sample input:
>   
>       user0 = [ "/nine.html", "/four.html", "/six.html", "/seven.html", "/one.html" ]
>       user1 = [ "/one.html", "/two.html", "/three.html", "/four.html", "/six.html" ]
>       user2 = [ "/nine.html", "/two.html", "/three.html", "/four.html", "/six.html", "/seven.html" ]
>       user3 = [ "/three.html", "/eight.html" ]
>   
>       Sample output:
>   
>       (user0, user2):
>          /four.html
>          /six.html
>          /seven.html
>   
>       (user1, user2):
>          /two.html
>          /three.html
>          /four.html
>          /six.html
>   
>       (user0, user3):
>          None
>   
>       (user1, user3):
>          /three.html
>   
>       Test cases:
>
>       List<String> user0 = Arrays.asList(
>           "/nine.html", "/four.html", "/six.html", "/seven.html", "/one.html" );
>       List<String> user1 = Arrays.asList(
>           "/one.html", "/two.html", "/three.html", "/four.html", "/six.html");
>       List<String> user2 = Arrays.asList(
>           "/nine.html", "/two.html", "/three.html", "/four.html", "/six.html",
>           "/seven.html");
>       List<String> user3 = Arrays.asList("/three.html", "/eight.html");

    private static Map<String, Integer> countDomains(String[] counts) {
      Map<String, Integer> map = new HashMap<>();
      for (String count : counts) {
        String[] parse = count.split(",");
        int num = Integer.parseInt(parse[0]);
        String[] domain = parse[1].split("\\.");
        //mobile.sports.yahoo.com
        for (int i = 0; i < domain.length; i++) {
          StringBuilder sub = new StringBuilder();
          for (int j = i; j < domain.length; j++) {
            sub.append(domain[j] + ".");
          }
          String subDomain = sub.toString().substring(0, sub.length() - 1);
          map.put(subDomain, map.getOrDefault(subDomain, 0) + num);
        }
      }
      return map;
    }

現場compile過，也過了test case，結果還是拒了。


<a name="datahero"></a>
### **DataHero** (\< 10 employees)
#### _CS forward email | Front end intern_

透過系上郵件得知這個實習機會，寄信過去，收到一個簡單的take home assignment，我覺得還挺有趣

1. Sign-up for a Free Trial DataHero account at https://datahero.com
    * Go through the onboarding process, upload a CSV data file of your choice, and create a chart. Write your name in the Subtitle of the Chart.
    * Export the chart to your computer and send the Chart as an attachment to your answers, as proof of your successful completion.
2. What could be improved about your experience using DataHero?
	* What is the highest priority feature you would improve about the product?
	* What area of the product would you most like to explore or improve during your internship?
3. Choose one of the following development tasks and write in words how you would approach completing the task. No need to write any code, just want to understand your thought process:
    * Enable embedding of charts on 3rd party websites:
	    - Allow charts to be embedded on public websites. We currently give users the ability to share charts by email or by link. Enable javascript snippets to allow users to share charts by embedding javascript code on 3rd party websites.
        - Anything to consider given our current sharing process?
    * Enable google auth for sign-up process:
        - Allow users to sign-up for DataHero using Google Auth. Take advantage of the passport package in npm
		- https://www.npmjs.com/package/passport-google-auth
        - Anything to consider given our current login process?
    * Add Twitter Ads API as a Data Connector:
		- Add Twitter Ads API as an additional DataHero data connector
		- https://developer.twitter.com/en/docs/ads/general/overview
		- Enable users to be able to connect to their Twitter Ads data to visualize their data using DataHero

寫完回覆後收到電面邀請

**CEO Phone Screening (Skype)**  
_30 mins_  CEO   
問了幾個題，純聊天，是個不到十人的小團隊，主要在講公司的營運以及做的產品，做business intelligence的東西，實習會寫NodeJS/ReactJS，但是沒辦法給很高的薪資。
然後讓我自介。面試完以後收到無聲卡，後來從面試它正職的朋友口中得知他intern就一口氣面了70個UCLA的學生。

<a name="nutanix"></a>
### **Nutanix** (3600 employees)
#### _內推 | ML/NLP intern_
_45 mins_ 印度小哥  
做Cloud Enterprise的公司，ML team會針對用戶使用系統的行為資料進行分析，比方說file system access, monitor anomoly behavior,，NLP的部分有兩個應用場景，一個是search query analysis，一個是document classification。

HR Screening
問了一下過去experience，我在被內推的時候並沒有選擇position，HR就說有新開一個ML/NLP position感覺跟我比較match，就幫我schedule了隔天給相關的team interview

Phone Interview 
印度人，給了一個coding的連結，結果全部都問觀念，focus on ML, python language and OS concepts
* given two python list with unsorted integers, return same elements
* do you have experience on writing ML algorithm from scratch? 
* explain OS memory management 
* explain OS page concepts
* any experience in cloud computing, parallel?
* any experience in virtual machine?
* explain pandas / numpy / python built-in list

- - - 
<a name="finance"></a>
## 三、Financial Firm

<a name="sga"></a>
### **Strategic Global Service**
#### _CS tea time | NLP intern_
在LA的New Port Beach投資公司。tea time時來系上招人，說需要懂NLP的來做intern，會做news trending方面的分析。我趕緊抱著履歷上前跟來的人聊我的NLP相關經驗。後來有一天我就直接收到了他們家的offer......，連正式面試都沒有。神奇的是package還不算太糟，$500 sign up fee, $1500/week, $500 - $2000 bonus，查了一下LinkedIn profile還有公司營運狀況也還行，但還是覺得這種招聘方式不太妥，想說之後應該能拿到別的公司，就先拒了offer。

<a name="deshaw"></a>
### **D.E.Shaw**
#### _海投 | Software Development Engineer Intern_
D.E.Shaw是在紐約的一家Hedge fund，除了software engineer，其餘員工基本上都是PhD degree

**Phone Interview**
_1 hour_ 美國大哥  
Introduction. He introduced himself, and then let me introduce my previous experience. He asked me further about the machine learning internship expericen and how I implemented deep learning algorithm.
> python knowledge

* tuple concept
* difference between list and tuple? 
* which is more memory waste? 
* why need tuple? 
* could list or tuple be key of dictionary?

> data structure concept

* given streaming data and maintain top 10 values. use PriorityQueue
* follow up: how heap works? MaxHeap/MinHeap, remove/add operation time complexity

> Math

* R square concept. use x1 to predict y. Now use x1 and x2 to predict y, does R square become larger or smaller?

由於家裡環境太糟，我到學校圖書館(Powell)的空教室面試，結果因為沒預約，被問最後一道題的時候有人進門說他們預約了，我只能邊收東西邊面試最後一題，邊慌亂的走出來，結果當然是被慘拒了。

<a name="row"></a>
### **ROW Asset Management**
約十人左右的quant company，總部在NYC。

#### _CS eamil | Python Distributed Developer Intern_
_1 hour_ 印度小哥  
MFE有個quant night，系上寄信給CS student說有這個position，我就立刻寄信，不到一小時就收到了面是邀請。

**On Campus Interview (Anderson classroom)**  
互相自介。
> print out the power set (all subsets) of an integer set  

叫我現場用自己的編輯器coding，說了句：「people always say someting on their resume, but the best way is letting them code」，非常嗆，我就毫不猶豫的用VIM快速寫了個Java的DFS解法並且過test case。然後它就給了一個python的快速解法，用integer存，但是我點出了前提得要set S的power set 不能超過2^32個可能。他說很不錯可以這麼短時間寫出來，可惜他們徵的是python developer，所以就不是很match。  

> 各種OS concepts，e.g. process v.s. thread?

- - - 
<a name="oversea"></a>
## 四、海外

<a name="tencent"></a>
### **Tencent 中國騰訊**
#### _海投 | NLP技術研究實習_
**On Campus (USC Leavey Library)**
一進門問好不到三十秒，國人小哥就拿了張紙條出來說，先做一下這道題吧

    Input: 2 integer arrays
    array 1 = [5, 3, 2, 2, 1, 3, 4]
    array 2 = [2, 1, 3]
    Output: 第一個數組按照第二個數組的順序排序，第二個數組沒出現過的放後面就可
    [2, 2, 1, 3, 3, 4, 5] or
    [2, 2, 1, 3, 3, 5, 4]
    Solution: LinkedHashMap

我們再來看一下這道題

    Leetcode 417. Pacific Atlantic Water Flow

**HR phone interview**


<a name="sea"></a>
### **SEA**
#### _Recruiter LinkedIn 聯繫 | Software Development Engineer Intern_
新加坡的公司，Garena前身，所有面試問最難的公司
HR Screening (Skype)
說明了有三個組，mobile development, backend, Shopee Search team
1st phone interview

- - - 

## 五、OA/ Take Home Assignment

<a name="ebay"></a>
### **eBay**
#### _Take Home | Data Science Inern_

<a name="twitter"></a>
### **Twitter**
#### _OA | Software Development Engineer Intern_

<a name="citadel"></a>
### **Citadel**
#### _OA | Software Development Engineer Intern_

<a name="squarespaece"></a>
### **Squarespace**
#### _Take Home | Data Science Inern_

<a name="adobe"></a>
### **Adobe**
#### _Take Home | Data Science Inern_
