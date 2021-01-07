+++
title = "Hugo 學習日誌01"
date = 2020-12-29T23:57:35+08:00
description = ""
tags = ["Hugo","網站架設"]
+++

>本站是透過**Hugo**這個靜態網站生成器製作而成的<br>
網路上還有其他的靜態網站生成器<br>
而我會選擇用**Hugo**的原因就是因為它安裝簡單生成快速<br>
我這裡只記錄怎麼用**Hugo**製作靜態網站跟我遇到的問題<br>
其他更詳細的內容請再上網搜尋
<!--more-->
## (一)安裝 **Hugo**
>說是安裝 **Hugo** 其實只需要一個 **hugo.exe** 就可以執行<br>
所以只要去&nbsp;&nbsp;[_**Hugo官網下載**_](https://gohugo.io/getting-started/installing)&nbsp;&nbsp;符合你電腦環境的執行檔就好</p>

![官網畫面](/github.io/image/Learn_Hugo/DownLoadHugo01.png)
>我是在 **Windows10&nbsp;x64** 系統環境下所以是載 
#### hugo_extended_<cite>(0.79.1)[^1]</cite>_Windows-64bit.zip
>將檔案解壓縮後就會得到一個&nbsp;**hugo.exe**<br>
其實現在就可以執行 **Hugo** 了，但是只能在目前解壓縮出來的目錄下<br>
為了之後執行方便，我建議修改<cite>環境變數&nbsp;[^2]</cite><br>
讓 **Windows PowerShell** 或 **Cmd** 不管在哪都可執行 **Hugo**<br>

![環境變數位置](/github.io/image/Learn_Hugo/DownLoadHugo02.png)
![新增環境變數](/github.io/image/Learn_Hugo/DownLoadHugo03.png)
>照著圖片操作最後按下確認就完成 **Hugo** 的安裝<br>
這時候可以打開 **Cmd** 來確認，執行指令 `hugo version`<br>
可以看到版號就代表成功了

![CMD驗證](/github.io/image/Learn_Hugo/DownLoadHugo04.png)
[^1]:看目前**Hugo**最新是哪一版。
[^2]:(Windows)作業系統會依照**PATH**環境變數中所設定的路徑順序，依序尋找各路徑可以執行命令的執行檔。
## (二)創建一網站
> 在確認**Hugo**可以執行後，下一步就是創建一個網站<br>
> 在你想要放網站檔案的位置開啟**Windows PowerShell**<br>
> 執行指令`hugo new site (Name)`
> ，**Name** 為你網站要取的名稱

![創建網站](/github.io/image/Learn_Hugo/CreateNewSite01.png)
>執行完畫面會如上圖，同時也會建出一個名稱 **(Name)** 的資料夾<br>
你會注意到 **Windows PowerShell** 其實也會指示你接下來要怎麼做<br>
所以我們就依照它的指示先去&nbsp;[**https://themes.gohugo.io/**](https://themes.gohugo.io/) 去選擇我們主題<br>
每個主題都可以點進去看，選擇自己喜歡的主題去下載<br>
按下 **Download** 後，會到這個主題的 <cite>**GitHub**[^3]</cite> 頁面<br>
直接點選 **Download&nbsp;&nbsp;ZIP** 下載就好

![GitHub下載](/github.io/image/Learn_Hugo/CreateNewSite02.png)
>下載完將 **ZIP** 檔名後面的`-master`刪除<br>
再放到剛創建 **(Name)** 的資料夾裡的 **themes** 資料夾下並解壓縮

![Hugo site 資料夾](/github.io/image/Learn_Hugo/CreateNewSite03.png)
>解開後你通常可以看到一個叫 **exampleSite** 的資料夾<br>
將裡面的檔案複製下來，回到 **(Name)** 的根目錄將它們貼上<br>
理論上這樣網站就已經有一個雛型了<br>
這時在 **(Name)** 的根目錄開啟 **Windows PowerShell** <br>
執行指令`hugo servver`後，你就可以在 [**http://localhost:1313/**](http://localhost:1313/)看到目前在本機運行的網站

![Hugo server](/github.io/image/Learn_Hugo/CreateNewSite04.png)
#### 可能遇到的問題
1.  `hugo servver`執行時出現Error，而不會出現上面的圖<br>
-    我遇到的問題之一，他顯示說我的主題太舊現在不支援，後來換一個主題就好了，所以在選主題時要注意它是否太久沒更新<p>
2.   連到 **http://localhost:1313/** 顯示不出網站來
-    我遇到的問題之一，我一開始用 Google chrome 會無法顯示，換個瀏覽器(Firefox, Edge)就好了 <p>  
3.   其他問題
-    因為每個主題都有不同的格式，所以可能還有其他要求才能執行網站，下載主題前可以先看主題下方的描述或解壓縮完的ReadMe的檔案，通常都會有作者的提示怎麼使用他的主題
[^3]:簡單來說就是儲存紀錄各種程式碼和檔案的網站，建議沒有帳戶可以去 [_**GitHub**_](https://github.com/) 註冊，方便管理你之後網站的檔案，同時也能讓你的網站上線。
## (三)創建文章
hugo new post/文章標題.md -> 創建一個新的文章</p>

