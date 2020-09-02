# Build_Our_Own_Speed_Test

# It a old collect bandwidth speedtest tool project , at 2016/04/08  #

Project  # Build_Our_Own_Speed_Test 0.0.0 # include:

1.WNMP (Nginx , MairaDB , PHP ) [1]、 FireZilla FTP Server ( Portable ) [2] , Dummy Test files (10M,100M,1000M  

2.incloude test bandwidth WEB TEST like :SPEEDTEST MINI[3] (Adobe Flash base speedtest , expired) , HTML5speedtest [4] 、 speedtest.js[5] 

3.tools: iPERF [6] base lazyScript , TFGEN in ( 中文 Chinese Traditional ) [7] , FileZilla FileFTP Client [7]  , NetMeter

4.FAQ

# Screenshot.png #

#REF: 
1.https://github.com/wnmp/wnmp/releases

2.https://filezilla-project.org/download.php?type=server

3.https://www.speedtest.net/mini

5.https://www.fast-air.net/speedtest/

.TFGEN 0.7 Tfgen traffic generator vers 0.7 Copyright (C) 1996-1997 K.YumotoChinese , A good traffic (unicast, multicast and broadcast)generator for testing.
Tfgen traffic generator vers 0.7 , http://afeng.logdown.com/posts/732444-tfgen-traffic-generator-chinese-version

6.https://iperf.fr/

6.https://filezilla-project.org/

7.NetMeterEvo,https://netmeter-evo.en.lo4d.com/windows


---------------------
#中文 Chinese Traditional 
測速懶人包 V0.0 afeng 20160408


By WNMP (Nginx , MairaDB , PHP ) & Firezilla FTP Server

###安裝及使用方式:
解壓縮檔案到 D:\Project_SpeedTest\

###WEB 網頁伺服器: 

執行
D:\Project_SpeedTest\Wnmp-2.2.3\Wnmp\Wnmp.exe

#網頁伺服器跟目錄:
D:\Project_SpeedTest\Wnmp-2.2.3\Wnmp\html

###FTP 伺服器:
#路徑:
D:\Project_SpeedTest\FileZilla Server

#FTP路徑
D:\Project_SpeedTest\FTPHOME 為 FTP 根目錄 (ROOT) 資料夾
D:\Project_SpeedTest\FTPHOME\UPLOAD 為 FTP 上傳資料資料夾

#FTP 管理程式:
FileZilla Server Interface.exe

#預設帳號密碼:
帳號:speed
密碼:SpeedTest1o5o4
權限:/ 可下載 10MB~1GB 檔案做下行測試
     /upload 可上傳/刪除檔案做上行測試

FileZilla FTP Server 免安裝版
# 啟動Server
"FileZilla Server.exe" /compat /start

#關閉Server
"FileZilla Server.exe" /compat /stop

###以下要有管理員權限###
#安裝服務
"FileZilla Server.exe" /install

#解除服務
"FileZilla Server.exe" /uninstall

#自訂服務名稱(注意 FileZilla Server.XML 可以讀寫)，執行檔可以複製更改名稱為喜歡的名字
"5566Server.exe" /servicename 5566FTPD
"5566Server.exe" /servicedisplayname 5566 FTP SERVER Service
"5566Server.exe" /install

#
FileZilla Wiki - Command-line arguments (Server) ,https://wiki.filezilla-project.org/Command-line_arguments_(Server)

#啟動 FTP 伺服器:
Lazy - 1.啟動 FTP Server.cmd

#關閉 FTP 伺服器
Lazy - 2.關閉 FTP Server.cmd

#安裝成服務(背景自動執行)
Lazy - 3.安裝為服務(需要管理員權限).cmd

#移除服務
Lazy - 4.解除系統服務(需要管理員權限).cmd

###FAQ
Q1:想放別的路徑可以嗎?
A1:可以啊，有路徑綁定的只有 FTP 伺服器，修改方式如下:
1.開啟 FileZilla Server\FileZilla Server.xml
2.找到 <Permission Dir="D:\Project_SpeedTest\FTPHOME"> 跟 <Permission Dir="D:\Project_SpeedTest\FTPHOME\UPLOAD">
3.將引號裏頭的路徑，更改為正確路徑就可以囉

Q2:我不想用預設帳號可以嗎?
A2:可以參考網路上相關的 Filezilla ftp server說明，透過 FileZilla Server Interface.exe Server 管理程式，去編輯使用者帳號或權限即可。

Q3:Speedtest mini 顯示過期?
A3:下載 http://c.speedtest.net/mini/mini.zip ，
然後把裡頭的檔案整個複製到 D:\Project_SpeedTest\Wnmp-2.2.3\Wnmp\html\mini 裡頭，並取代及可。

---
#REF: 
1.https://github.com/wnmp/wnmp/releases

2.https://filezilla-project.org/download.php?type=server

3.https://www.speedtest.net/mini

5.https://www.fast-air.net/speedtest/

.TFGEN 0.7 Tfgen traffic generator vers 0.7 Copyright (C) 1996-1997 K.YumotoChinese , A good traffic (unicast, multicast and broadcast)generator for testing.
Tfgen traffic generator vers 0.7 , http://afeng.logdown.com/posts/732444-tfgen-traffic-generator-chinese-version

6.https://iperf.fr/

6.https://filezilla-project.org/

7.NetMeterEvo,https://netmeter-evo.en.lo4d.com/windows
