+++
title = "第一篇文章"
date = 2020-12-27T20:09:35+08:00
description = "紀錄如何使用Markdown來寫網頁內容"
tags = ["Markdown","網站架設"]
+++

Markdown的網頁文字範例</p>
主要用來測試用的</p>

<!--more-->

## 設置文字大小

用 `#` 的數量來同等於 HTML的 `<h1>`—`<h6>`</p>

# H1

## H2

### H3

#### H4

##### H5

###### H6


## 標記文字方式透過 `註解` , `粗體` 或 `斜體` 

#### 文字中標記方式

> 文字要分段時，可以用HTML的 `</p>`</p>
> 文字要換行時，可以用HTML的 `<br>`<br>
> 文字中要插入&nbsp;空&nbsp;白&nbsp;鍵&nbsp;時，可以用HTML的 `&nbsp;`<br>
> 用 **星號** 標記粗體，用 _底線_ 來標註斜體，注意底線不要跟前後文字相連<br>
> 同時要用 **_粗斜體_** 時，星號一定要加在底線外

#### 標記註解的方式

> 透過 `<cite>` 跟 `</cite>` 將想要註解的文字夾起來，並在裡面用 <cite>中括號&nbsp;[^1]</cite>&nbsp;來決定註解代號<br>
> 但是要注意代號不等於右上 <cite>註解&nbsp;[^a]</cite>&nbsp;的數字，而是要配對註解用的

[^1]:寫法是[^代號]
[^a]:註解的數字是自動按照順序排的，而且被註解的文字會自動變斜體

## 表格
| Name  | Age |
| ----- | --- |
| Bob   | 27  |
| Alice | 23  |
| John  | 30  |

表格中也能用前面介紹的文字標記</p>

| Online|Markdown |    In     | Table  |
| ------|-------- | ----------| ------ |
| _斜體_|**粗體** |~~刪除線~~ | `標記` |

## 列目錄

#### <cite>數字目錄&nbsp;[^2]</cite>
[^2]:第一個數字決定從哪個數字開始數直到目錄結束，後面的目錄數字在Markdown不影響網頁顯示
1. 第一個項目
6. 第二個項目
4. 第三個項目

#### 純目錄

-   一個物件
-   另一個物件
-   再一個物件

 #### 混和目錄

-   一個物件
2.  第二個目錄
5.  我不是三
-   4. 羅馬數字目錄
7.  第三個目錄

## 程式顯示
```html
html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>Example HTML5 Document</title>
    </head>
    <body>
        <p>Test</p>
    </body>
</html>
```
``` C
c 語言
int a;
int b;

a = 1;
b = 2;

a = a + b;
```
## 其他元素 — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> 文字說明

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

按下<kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> 來結束目前的程式

重點會用<mark>螢光標示</mark>起來

## 圖片&影片顯示

#### <cite>本地圖片&nbsp;[^3]</cite>

![新年](/github.io/image/New_Year.jpg)

[^3]:注意圖片名不能有空格
#### 調整圖片大小
{{< figure src="/github.io/image/New_Year.jpg" width="50%" >}}

#### 網路圖片
![黃金神威網路圖](https://pbs.twimg.com/media/EqUV120UYAIJm9_.jpg)

#### 網頁超連結

[巴哈姆特](https://www.gamer.com.tw/)

#### YouTube 影片嵌入
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/c7vpcqA6SEQ?start=1700" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
