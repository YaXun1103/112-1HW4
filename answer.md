# 第4次作業-作業-HW4
>
>學號：111111109
><br />
>姓名：張雅薰
><br />
>作業撰寫時間：45 (mins，包含程式撰寫時間)
><br />
>最後撰寫文件日期：2023/12/22
>

本份文件包含以下主題：(至少需下面兩項，若是有多者可以自行新增)
- [x] 說明內容
- [x] 個人認為完成作業須具備觀念

## 說明程式與內容
先fork老師的倉庫並clone 
```
git clone
```
a.  若今天將兩個div的css中，各加上  border: 1px solid blue;  屬性與屬性值會發生什麼事情
```html
<style>
        .menu{
            float: left;
            background-color: #FF0000;
            min-width: 30%;
            border: 1px solid blue;
        }
        .contentContainer{
            float: right;
            background-color: #00FFFF;
            min-width: 70%;
            border: 1px solid blue;
        }
    </style>
```
![image](螢幕擷取畫面%202023-12-17%20181431.png)
b.要對兩者css要怎麼處理才能回復成p.37的div並排格式，列出程式碼後，說明想法 
```html
box-sizing: border-box;
```
在網路上搜尋css的排版方式看到可以使用box-sizing去控制元件的長寬範圍，分為:<br />
Content-box (寬高設定作用在內容範圍)<br />
Border-box （寬高設定作用在邊框外緣的範圍內）
![image](螢幕擷取畫面%202023-12-11%20164415.png)
c.  由左至右套用div的CSS類別分別. menu ,  .contentContainer , 與.functionContainer 且各自的min-width為30%, 50%與20%。根據上小題的
b的結果繼續實作成三欄式畫面。
```html
<div class="functionContainer">
        內容區塊
    </div>
```
```html
<style>
        .menu{
            float: left;
            background-color: #FF0000;
            min-width: 30%;
            border: 1px solid blue;
            box-sizing: border-box;
        }
        .contentContainer{
            float: right;
            background-color: #00FFFF;
            min-width: 50%;
            border: 1px solid blue;
            box-sizing: border-box;
        }
        .functionContainer{
            float: right;
            background-color: #00FFFF;
            min-width: 20%;
            border: 1px solid blue;
            box-sizing: border-box;
        }
    </style>
```
![image](螢幕擷取畫面%202023-12-17%20201431.png)
推上github
```
git add 
git commit 
git push
```
## 個人認為完成作業須具備觀念

1.基本的Git操作:<br />
例如fork別人的倉庫、clone倉庫到本地、add、commit、push等基本的操作。<br />

2.box-sizing的運用：<br />
box-sizing對於網頁排版是至關重要的，特別是在設計多欄式畫面時。透過將 box-sizing 設為 border-box;，可以更直觀地控制元素的寬度和高度，確保邊框和內容都包含在指定的範圍內。<br />

3.CSS浮動及並排結構的理解:<br />
使用float屬性能夠實現元素的並排顯示，結合 float與 box-sizing，能夠輕鬆地配置多個區塊，使其在同一行上並排呈現。<br />

