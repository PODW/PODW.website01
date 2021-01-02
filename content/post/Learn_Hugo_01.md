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
>說是安裝**Hugo**其實只需要一個**hugo.exe**就可以執行<br>
所以只要去&nbsp;&nbsp;[**Hugo官網下載**](https://gohugo.io/getting-started/installing)&nbsp;&nbsp;符合你電腦環境的執行檔就好</p>

![官網畫面](/github.io/image/Learn_Hugo/DownLoadHugo01.png)
>我是在`Windows10`&nbsp;**x64**系統環境下所以是載 
#### hugo_extended_<cite>(0.79.0)[^1]</cite>_Windows-64bit.zip
>將檔案解壓縮後就會得到一個&nbsp;**hugo.exe**<br>
其實現在就可以執行**Hugo**了，但是只能在目前解壓縮出來的目錄下<br>
為了之後執行方便我建議把修改<cite>環境變數&nbsp;[^2]</cite><br>
讓**Windows PowerShell**或**Cmd**不管在哪都可執行**Hugo**<br>

![環境變數位置](/github.io/image/Learn_Hugo/DownLoadHugo02.png)
![新增環境變數](/github.io/image/Learn_Hugo/DownLoadHugo03.png)
>照著圖片操作最後按下確認就完成**Hugo**的安裝<br>
這時候可以打開**Cmd**來確認，執行**hugo&nbsp;&nbsp;version**<br>
可以看到版號就代表成功了

![CMD驗證](/github.io/image/Learn_Hugo/DownLoadHugo04.png)
[^1]:看目前**Hugo**最新是哪一版
[^2]:(Windows)作業系統會依照**PATH**環境變數中所設定的路徑順序，依序尋找各路徑可以執行命令的執行檔
## (二)創建一網站

hugo server -> 運行本機的server來顯示目前的網頁</p>

hugo new site 名稱 -> 創建一個新的網站</p>

hugo new post/文章標題.md -> 創建一個新的文章</p>

hugo -> 將目前製作的網頁輸出成 html