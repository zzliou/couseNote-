# couseNote- 
2023.11.4
“專案”會說repo 比較口語

要打出字的步驟
1.<h1 class="title">hello world</h1>

要更改字體顏色步驟
1. 建立ＣＳＳ檔
2.ＣＳＳ檔案內加入.title{
    color:blue;
}
3. 在html檔案中的head 底部 加入<link rel="stylesheet" href="./style.css">
回到html檔案開啟即完成
   ＰＳ． rel也可以改成icon ....等等

2023.11.6
今天開始學刻unote的navbar
margin-left margin-top margin-right 
前端工程師思維 ： 一組一組往下包‘ 可以用不到 但避免要用的時候沒包到,導致重寫
字體加在：head那包, 到google fonts 找連結複製貼上‘到ＣＳＳ要加font-family:'字體ａ','字體Ｂ‘;>> ＣＳＳ是告訴軟體要使用這個字體！

2023.11.7 
刻出unocha 的header了

2023.11.8
font: 400=normal 700=bold 
文字的置左:text-align: left; 、置中: text-align: center; 、置右: text-align: right;
在容器中的置中 
.container {
    display: block;
    width: 1070px;
    margin: 0 auto; →(如果寬度不夠佔據一整行,剩下的空隙 margin會自動補, )
    }

2023.11.11
今天把LOGO放上去, 用到 display:flex 這個語法, "彈性"
.header .navbar {
  display: flex; -> 彈性
  align-items: center; -> 上下置中 
align 上下 justify 左右 
是排版很重要的招數 
EX: 兩個區塊不想同時靠左或靠右, 把其中一個區塊下margin-left/right: auto 即可解決

2023.11.12
position 
有分成static (預設值)、absolute (絕對配置)、relative (相對配置)、fixed (固定配置)

position: fixed　固定配置 :將元素固定在某個地方 →滑網頁的時候他都會固定出現在某個地方 
 .oder-button-container {
    position: fixed;
    right: 100px;　位置要擺哪裡
    bottom: 50px;
    background-color: white; 　底色
    width: 100px;　　大小
    height: 100px;　　
    border-radius: 50px; -> 邊框圓角
    padding: 20px;　
    width: 50px;　正圓
    height: 50px;
    border: solid #eed7b0;　外框的樣式跟顏色
}

更複雜的版面配置用
 * 一個用position: relative ←→　另一個就要用position: absolute
因為是相呼應的元素才會喚起這兩個功能!

.oder-button-container .wrapper {             記得創一個ｃｌａｓｓ作為相對配置的母------------> 
    position: relative;
    width: 100px;
    height: 100px;
}

.oder-button-container .wrapper .oder-cute-image {　　　子
    position: absolute;
    width: 60px;
    right: 8px;
    bottom: 0px;  如果沒有差太多,沒有更改到bottom 還是要放0 , 把它keep住, 免得換了不同版面會跑掉
}

.oder-button-container .wrapper .oder-text-image {　　子　
    position: absolute;
    width: 20px;
}

2023.11.16
table 
tr = table row & td = table data 
也可以用 thead tbody tfoot 
Form


 
