---
layout: post
title: 2018北美實習面經
---

近年CS求職難度越來越大，找實習的過程很艱辛，但也受到很多人幫助、鼓勵，因此想要回饋一下，分享給需要的朋友們。  

這邊整理了我在找2018 summer intern面試的17家公司，接近30輪interviews，還有4家OA/Take home assignment。先分類、再按照面試時間排序。



<!-- more -->

1. <a href="#big">大公司</a>
    * 10.25 <a href="#microsoft">Microsoft</a> 
    * 12.13 <a href="#google">Google</a> 
    * 12.20 <a href="#salesforce">Salesforce</a>
    * 01.25 <a href="#linkedin">LinkedIn</a>
    * 02.14 <a href="#intel">Intel</a>
    * 02.16 <a href="#paypal">PayPal</a> (offer)
2. <a href="#startup">中小型 & 新創</a>
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
    * <a href="#ebay">eBay</a>
    * <a href="#adobe">Adobe</a>
    * <a href="#twitter">Twitter</a>
    * <a href="#citadel">Citadel</a>

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

面試Research intern前，HR會給一個問卷讓你提供你的研究方向，我當時是選NLP，結果他幫我schedule了一個CV方向的人面我，於是我趕緊寄信讓他更正。有簽了NDA就不透漏太多了，一輪問研究經驗，一輪純寫代碼，考了LC原題。

比較值得一題的是第二輪的溝通。面我的是大家普遍最怕的印度工程師，雖然從一開始他除了講的，也還會把所說的重點打在Google doc上。但我剛來沒多久印度腔還很不適應，對方語速也偏快，中間好幾次聽不清楚還是得請他重講。建議來美國多跟印度人講話或是至少聽他們說話，熟悉一下印度腔。另外一點就是因為問了原題，我一開始就給了最優解，沒有先給一個較差但直覺的解法，他就說他看不出來為何要用這個最優的解法，說你要不要先從簡單的開始。雖然最後還是寫了最佳解，但溝通並不是非常順暢，一週後跪了。所以交流很重要。一個練習電面的方法是平常刷題時邊寫邊think out loud，會更像真實面試情境。

此外我在一開始還遇到一個插曲，面試官電話打不進來，晚了快十分鐘才面試，後來發現家裡收訊太差，所以電面的時候除了要找個安靜的地方，還要注意一下手機收訊，避免跟我一樣白白少了十分鐘面試時間。

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
HR來信，主要考點：
- 算法、CS基礎
- 解釋、實作code，不用IDE以及online docs
- DBMS基礎知識以及架構

**1st phone interview (collabedit)**  
_1 hour_ 中國小哥 Senior SDE  

> 利口餓零靈，小島數量

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

> 利扣惡傘溜，二搜樹最小共同祖先

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

> Q1: Returns true if the input string is a number and false otherwise. For example +1 ,-1 ,1.0, 32, .2 

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
                char ch = toTest.charAt(i);
                if (i == 0 && ch == '+' || ch == '-') continue;
                if (toTest.charAt(i) == '.') {
                    if (sign) return false;
                    else sign = true;
                }
                else if (ch >= '0' && ch <= '9') continue;
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

最後他說希望我能加入LinkedIn，會給我寫strongly recommend to recruiter。面試完相當激動，覺得努力很久終於有收穫了，唯一一個可能就是提前招滿，但是HR跟我schedule interview的時候說這個position才剛開始招，感覺很穩了。

過幾天後HR打來說你的feedback positive但招滿了。。。。。。打擊非常大，完美面試、交流順暢，還能被拒，發文討拍後move on繼續面其他間。

<br>
#### _內推 | Data Science, Analytic Intern_ 
HR來信說明面試範圍：problem solving問題，主要會是領英實際面對的business case study；解題的時候看重使用的framework, assumptions, communication，請有細節的使用analytical approach還有步驟並且引導出最終結論。為了了解你怎麼reason with mathematical concepts and inferences，也會考applied statistics/machine learning/probability theory to business problems. 

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
這邊我用MECE框架，一個consulting company常用的解決問題模型。

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

A/B testing完全沒學過、統計很多也忘光光，直接跪了。

### **Intel**
#### _Info Session_  
Intel比較特別，幫軍方做chips，所以對於身分要求很高，查很嚴，只有很少數的人能拿到面試。我在Info session後與裡面的人聊聊，首先就先被問是不是公民，然後說Intel的IT department只收公民，其他的department就沒這個要求。然後跟一個中國大哥聊聊，說自己本來想讀PhD但後來放棄，就說我可以跟你聊聊，要不約個明天吧？蠻妙的竟然是這個原因拿到on campus。  

**on campus (UCLA Career Center)**   
_1 hour_ 中國大哥  
沒有任何的coding，或是技術問題，一小時都是聊天。聊一下我的興趣、做的研究、為什麼想做研究，然後大哥解釋了他們想招的人，是audio signal processing engineer，但是想要用deep learning技術來做，聊了一下產品，還有哪些可能跟我可以做的項目。最後他講他當時讀博到一半quit的故事，鼓勵我如果可以的話，考慮一下讀博哈哈。然後說他會把我推薦給組內還有其他組看有沒有機會match。

然後就沒下文了。

### **PayPal**
#### _海投 | Cloud Engineer Intern_
Qualified candidate should be good at using problem solving skills, algorithms and data structures to use machine learning for our platform.  
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
> 力扣夭兩腰，買賣股票最佳時機

遇到插曲，collabedit網站掛掉寫不了code，我就在skype上面打一行說明一行，而且還沒有縮排，但還是有解釋清楚。

> Q2: implement Binary Search

此時colladbedit還是爛掉，於是也只能在skype messege裡敲代碼，這邊我用這個<a href="http://community.bittiger.io/topic/241/一起lintcode-二分查找看这篇就够了">binary search系列模版</a>

    public int bsearch(int[] nums, int target) {
        if (nums.length == 0) return -1;
        int start = 0, end = nums.length - 1;
        // 不用start < end 是為了避免有些情況會infinite loop
        while (start + 1 < end) {
            // 這邊跟面試官解釋了
            // integer overflow problem using mid = (start + end) / 2
            int mid = start + (end - start) / 2;
            if (nums[mid] == target) return mid;
            else if (nums[mid] < target) start = mid;
            else end = mid;
        }
        // 改良start + 1 < end後的二次判定
        if (nums[start] == target) return start;
        if (nums[end] == target) return end;
        return -1;
    }

> Q3: 各種Java觀念
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

> 裡叩叭妖腰，次網域拜訪次數

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
          String subDomain = sub.toString().substring(0, sub.length()-1);
          map.put(subDomain, map.getOrDefault(subDomain, 0) + num);
        }
      }
      return map;
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
做Cloud Enterprise的公司，最近成長勢頭很強。ML team會針對用戶使用系統的行為資料進行分析，比方說file system access, monitor anomoly behavior,，NLP的部分有兩個應用場景，一個是search query analysis，一個是document classification。

**HR Screening**  
問了一下過去experience，我在被內推的時候並沒有選擇position，HR就說有新開一個ML/NLP position感覺跟我比較match，就幫我schedule了隔天給相關的team interview

**1st Phone Interview**  
_45 mins_ 印度小哥   
給了一個coding的連結，結果全部都問觀念，focus on ML, python language and OS concepts
* given two python list with unsorted integers, return same elements
* do you have experience on writing ML algorithm from scratch? 
* explain OS memory management 
* explain OS page concepts
* any experience in cloud computing, parallel?
* any experience in virtual machine?
* explain pandas / numpy / python built-in list

自己覺得回答的挺差的，想不到move forward了

**2nd Phone Interview**  
on going

- - - 
<a name="finance"></a>
## 三、Financial Firm

<a name="sga"></a>
### **Strategic Global Service**
#### _CS tea time | NLP intern_
在LA的New Port Beach投資公司。tea time時來系上招人，說需要懂NLP的來做intern，會做news trending方面的分析。我趕緊抱著履歷上前跟來的人聊我的NLP相關經驗。後來有一天我就直接收到了他們家的offer，連正式面試都沒有。儘管給的package不差，查了一下LinkedIn profile還有公司營運狀況也還行，但還是覺得這種招聘方式不太妥，怕怕的就沒有接下offer。

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
#### _CS eamil | Python Distributed Developer Intern_
約十人左右的quant company，總部在NYC。MFE有個quant night，系上寄信給CS student說有這個position，我就立刻寄信，不到一小時就收到了面試邀請。

**On Campus Interview (Anderson classroom)**  
_1 hour_ 印度校友  
互相自介。
> Q1. SQL concept. Update a table using nested query

> Q2. print out the power set (all subsets) of an integer set S

叫我現場用自己的編輯器coding，說了句：「people always say someting on their resume, but the best way is letting them code」，非常嗆，我就毫不猶豫的用VIM快速寫了個Java的DFS解法並且過test case。然後它就給了一個python的快速解法，用integer存，但是我點出了前提得要set S的power set 不能超過2^32個可能。他說很不錯可以這麼短時間寫出來，可惜他們徵的是python developer，所以就不是很match。  

> Q3. 各種OS concepts

* process v.s. thread?
* inner process communication
* deadlock

- - - 
<a name="oversea"></a>
## 四、海外

<a name="tencent"></a>
### **Tencent 中國騰訊**
騰訊很用心，派了大批人馬來北美各大城市名校招聘實習生。全程中文面試，倍感親切。

#### _海投 | NLP技術研究實習_
**On Campus (USC Leavey Library)**  
_1 hour_ 中國大哥  
一進門問好不到三十秒，小哥就拿了張紙條出來說，先做一下這道題吧

    Input: 2 integer arrays
    array 1 = [5, 3, 2, 2, 1, 3, 4]
    array 2 = [2, 1, 3]
    Output: 第一個數組按照第二個數組的順序排序，第二個數組沒出現過的放後面就可
    [2, 2, 1, 3, 3, 4, 5] or
    [2, 2, 1, 3, 3, 5, 4]
    Solution: LinkedHashMap

過程中我詢問是否要think out loud，他說你全部寫完再跟我說。這點與美國面試相當不同。寫完後被問了複雜度，接著小哥從紙堆中又拿了一道題出來，「我們再來看一下這道題」

    李寇是妖妻，太平洋大西洋水流

半年多前做過這道，但忘了，跟面試官提出了幾個思路，被面試官說你再想一下，最後想出了解法並說明，但有點run out of time。所以剩下十分鐘就聊一下NLP research，我講解了一下deep learning model in coreference resolution。

**HR phone interview**  
_1 hour_ 中國姐姐  
* 為什麼會想來騰訊
* 對騰訊的了解
* 未來職涯規劃
* 美國的科技科研還是更前沿一點，為何要來我們這邊？
* 對加班的看法

<a name="sea"></a>
### **SEA**
#### _Recruiter LinkedIn 聯繫 | Software Development Engineer Intern_
新加坡的公司，Garena前身

**HR Screening (Skype)**  
說明了有三個組，mobile development, backend, Shopee Search team

**1st phone interview**

> Q1: Given an array of ints, and an integer n
> Find all distinct pairs of integers in the array that sum up to n
> 
> Example:
> [6,1,0,3,5,3,4,2,4,5]      n = 8
> Ans: [(3, 5), (4, 4)]     (4, 4), (3, 5)   (5,3)
> 
> Constraints
> - array is not sorted, can have duplicates
> - integers range from 0 to 2^32 - 1
> - length of array can be from 0 to 2^32 - 1
> - answer has distinct pairs
> - order inside the answer doesnt matter
> - optimise in terms of time and space complexity
> 
> Write a function to solve the problem
> input: int arr, int n
> output: list of pairs

    class Main {
        public static void main(String[] args) {
            System.out.println("Hello, world!");
        }
        // nums = [], nums = [0], num =[6,1,0,3,5,3,4,2,4,5] 
        public List<List<Integer>> pair(int[] nums, int n) {
            // space: O(N)
            Map<Integer, Integer> map = new HashMap<>();
            
            // time: O(N)
            for (int num: nums) {
                map.put(num, map.getOrDefault(num, 0) + 1);
            }
             
            // time: O(N)   
            List<List<Integer>> list = new LinkedList<>();
            for (Integer num: map.keySet()) {
                if (map.contains(n - num)) {        
                    if (num < n / 2 || num == n / 2 && map.get(num) > 1) {
                        // n = 8, num = 3, map contains 5
                        List<Integer> pair = new LinkedList<>();
                        pair.add(num);
                        pair.add(n - num);
                        list.add(pair);
                    }
                }
            }
            return list;
            
            // total time: O(N)
            // space: O(N)
        }
    }


> Q2: There are following two tables in a database.
> user_info table, which stores users' basic information. Structured as below:
> 
>         Field         Type              Description  
>       user_id          INT   ID of user(Primary key)
>     user_name  VARCHAR(32)                 username  
> 
> user_login_log table, which stores users' login records. Structured as below:
> 
>          Field       Type         Description  
>             id        INT         primary key  
>        user_id        INT          ID of user  
>     login_time   DATETIME  time of this login
> 
> Now please write a SQL statement to query user name and login count for all users who have logged in for more than 100 times in the year of 2014, and sort the query results by the login count in descending order:

    select user_name as Name, count(login_time) as Time
    from user_info I, user_login_log L
    where I.user_id == L.user_id && get_year(login_time) == 2014
    group by user_id
    having count(login_time) > 100
    order by count(login_time) desc
    

> Q3. How will database take use of composite index INDEX(a, b) in the "user" table for following queries?  
> A. SELECT * FROM user WHERE a=0 AND b=0;  
> B. SELECT * FROM user WHERE a=0 OR b=0;  
> C. SELECT * FROM user WHERE a>0 AND b=0;  
> D. SELECT * FROM user WHERE a=0 AND b>0;  

> Q4. OS concepts
* process vs thread
* context switch
* virtual memory
* mutex vs semaphore

    mutex true/false 
    semaphore counter
    if (mutex) {
       execute          
       mutex = false
    }  
    
    if (semaphore > 0) {
        execute
        semaphore--;
    }

> Q5. Network concepts
* tcp vs udp
* packets arrive in order

**2nd video interview**  
_1 hour_ Search team manager

> Leetcode 32. Longest Valid Parentheses

> Explain your NLP project. Why you use attention here......etc.

- - - 

<a name="oa"></a>   
## 五、OA/ Take Home Assignment

<a name="ebay"></a>
### **eBay**
#### _Take Home | Data Science Inern_
Finished Kaggle chanllege <a href="https://www.kaggle.com/c/DontGetKicked">"Don't Get Kicked"</a> and upload

<a name="adobe"></a>
### **Adobe**
#### _Take Home | Data Science Inern_  
給了一個data.csv，要從中create model to predict y，然後把model對test.csv的prediction回傳給HR

<a name="twitter"></a>
### **Twitter**
#### _OA | Software Development Engineer Intern_
有投就給OA，有六七組題庫隨機抽選一組，我拿到了OA Test 7，共三題，建議90 mins內完成
> 裡口舞芭武，在前年投資

> 忘了，easy 難度的題  

> 給一段密文，先用「肉眼」解密，之後再寫code用這組key解出密文輸出明文

<a name="citadel"></a>
### **Citadel**
#### _OA | Software Development Engineer Intern_
有投就給OA，考察範圍廣泛
* pandas library
    - cleaning up missing data
    - detect NaN
    - add new column
* math
    - which is larger ? max_x min_y f(x, y) v.s. min_y max_x f(x, y)
    - Guassian Distribution
    - homoskedastic error
    - probability question
* machine learning
    - perceptron convergence properties
    - hyperparameter search v.s. grid search
    - L0, L1, L2 norm
    - KNN algorithm
