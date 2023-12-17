# 第4次作業-作業-HW4
>
>學號：111111109
><br />
>姓名：張雅薰
><br />
>作業撰寫時間：35 (mins，包含程式撰寫時間)
><br />
>最後撰寫文件日期：2023/12/17
>

本份文件包含以下主題：(至少需下面兩項，若是有多者可以自行新增)
- [x] 說明內容
- [x] 個人認為完成作業須具備觀念

## 說明程式與內容

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

![image](螢幕擷取畫面%202023-12-11%20164415.png)

c.  由左至右套用div的CSS類別分別. menu ,  .contentContainer , 與.functionContainer 且各自的min-width為30%, 50%與20%。請根據上小題的
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


## 個人認為完成作業須具備觀念

開始寫說明，需要說明本次作業個人覺得需學會那些觀念，亦可作為學習筆記使用 (需寫成文章，需最少50字，並且文內不得有你、我、他三種文字)