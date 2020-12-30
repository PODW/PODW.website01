+++
title = "第一篇文章"
date = 2020-12-27T20:09:35+08:00
description = "紀錄如何使用Markdown來寫網頁內容"
tags = ["雜談","Markdown"]
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

> 文字要分行時，可以用HTML的 `</p>`</p>
> 用 **星號** 標記粗體，用 _底線_ 來標註斜體，注意底線不要跟前後文字相連</p> 
> 同時要用 **_粗斜體_** 時，星號一定要加在底線外

#### 標記註解的方式

> 透過 `<cite>` 跟 `</cite>` 將想要註解的文字夾起來，並在裡面用 <cite> 中括號[^1]</cite> 來決定註解代號</p>
> 但是要注意代號不等於右上 <cite>註解[^a]</cite> 的數字，而是要配對註解用的

[^1]:寫法是[^代號]
[^a]:註解的數字是自動按照順序排的，而且被註解的文字會自動變斜體

表格
| Name  | Age |
| ----- | --- |
| Bob   | 27  |
| Alice | 23  |
| John  | 30  |

本地圖片(注意圖片名不能有空格)
![新年](/image/New_Year.jpg)

調整圖片大小
{{< figure src="/image/New_Year.jpg" width="50%" >}}

網路圖片
![黃金神威網路圖](https://pbs.twimg.com/media/EqUV120UYAIJm9_.jpg)

網頁超連結

[巴哈姆特](https://www.gamer.com.tw/)

YouTube 影片嵌入
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/c7vpcqA6SEQ?start=1700" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


