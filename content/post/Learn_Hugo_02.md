+++
title = "Hugo 學習日誌02"
date = 2021-01-18T22:00:26+08:00
description = "Hugo的架構介紹跟實作"
tags = ["Hugo","網站架設"]
+++

>在前一篇文章介紹如何用 **Hugo** 創建簡易的網站<br>
這篇會介紹 **Hugo** 創建的網站裡各個資料夾的功用<br>
還有設定檔 `config.toml` 的介紹(以本站為範例)<br>
跟分享我自己摸索的一些實作
<!--more-->
## (一) **Hugo** 架構介紹
> 下圖為創建網站後的基本架構

![Hugo架構](/github.io/image/Learn_Hugo/HugoIntroduce00.png)
### **themes**
> 這個資料夾在創建網站時就用過了，就是拿來存放網站主題用的<br>
### **static**
> 這個資料夾是用來存放網站實體的資源，例如圖片等<br>
放在這個資料夾的資源，可以直接透過網站的根目錄找到實體，路徑等同於**static**裡的路徑<br>
所以在網頁裡要呼叫圖片時，也是用相同的路徑
### **resources**
### **layouts**
### **data**
>這三個我目前還不是很清楚要如何介紹，之後理解後會再補充
### **content**
> 這個資料夾就是存放各個網頁內容的地方，通常網誌的文章都放在 **post** 裡<br>
在來就看你所選的主題是否新增其他頁面，你覺得不夠也可以自己加
### **archetypes**
> 這個資料夾存放一個`default.md`的檔案，這是你每次在創建網頁文章的預設範本<br>
如果你覺得每次創建新的頁面都要重打一些重複內容很麻煩，你可以修改這個檔案
## (二) **config.toml** 的介紹
> 這個檔案其實就是這個網站的設定檔，可以透過修改裡面的參數來改造這個網站<br>
而每個不同的主題 **config.toml** 也會長的不一樣<br>
以下用這個網站的 **config.toml** 當範例

![Config範例](/github.io/image/Learn_Hugo/ConfigIntroduce00.png)
1. <mark>title</mark> 很明顯的是指網站的標題
2. <mark>theme</mark> 是指你主題的名稱，要注意 **themes** 資料夾內的主題名稱要跟這個相同才會認到
3. 這兩個項目是指網站預設的語系，不一定每個主題都會有這些項目，也不一定會有中文的選項<br>
這個我是看主題作者的介紹才知道這兩個參數可以調
4. <mark>subTitle</mark>就是指網站的副標

> 其實你可以對照模擬網站跟 **config.toml** 看這些參數對應網站那些資料<br>
> 直接嘗試修改 **config.toml** 並存檔，看網站因為你的修改而有哪些不同<br>
> 你也可以看 **config.toml** 的註解，通常會告訴你這些參數是在做什麼<br>

## (三) 實作案例
> 我這個主題有提供更換 _icon_ 的 _html_ (`favicon.html`)，放在 `/layouts/partials/` 底下<br>
> 而 `favicon.html` 內容如下

![Config範例](/github.io/image/Learn_Hugo/FaviconHtml00.png)
參考註解到 [**realfavicongenerator.net**](https://realfavicongenerator.net/) 這個網站可以將想要的圖片製作成 _icon_

## (四) 參考資料
>這是我學習的參考影片，如果看文字還是不了解的可以看看
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/c7vpcqA6SEQ?start=00" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>