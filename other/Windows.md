# Windows筆記

[Microsoft Security Bulletins](https://technet.microsoft.com/en-us/security/bulletins.aspx) Windows系統的安全性更新

##實用軟體
###網路
* [Firefox](http://moztw.org/firefox/download/latest-win.html)　網頁瀏覽器
* [PCMan](http://pcman.ptt.cc/)　BBS
* [FileZilla](https://filezilla-project.org/download.php?type=client)　FTP
* [MobaXterm](http://mobaxterm.mobatek.net/download-home-edition.html)　連SSH，也有FTP的功能
* [Comodo Firewall](https://www.comodo.com/home/internet-security/firewall.php)　免費防火牆
* [Avira Free Antivirus](http://www.avira.com/zh-tw/download-start-new/product/avira-free-antivirus)　免費防毒軟體
* [Adobe Flash Player](http://get.adobe.com/tw/flashplayer/)　不確定該歸類在網路還是多媒體下
* [Pale Moon](https://www.palemoon.org/)　網頁瀏覽器

###文書
* [Microsoft Office](https://office.com/start/default.aspx?WT.mc_id=Office_Products_site)　付費軟體，自然就沒有下載連結了XD。連結是免費線上版的。
* [Adobe Reader](http://get.adobe.com/tw/reader/)　看PDF用
* Adobe Acrobat　付費軟體，製做PDF用。
* [WinDjView](http://sourceforge.net/projects/windjview/)　看DjVu檔用

###多媒體
* [IrfanView](http://www.irfanview.com/main_download_engl.htm)　看圖軟體，附有簡單的圖像編輯功能
* [GIMP](http://www.gimp.org/downloads/)　免費圖像編輯軟體
* [Audacity](http://audacity.sourceforge.net/download/?lang=zh-TW)　免費音訊編輯軟體
* [MPC-HC](http://mpc-hc.org/)　看影片，支援多種格式

###文字編輯器
* [Notepad++](http://notepad-plus-plus.org/download/)　高級版記事本

###檔案驗證
* [File Checksum Integrity Verifier](https://support.microsoft.com/en-us/kb/841290)
* [Get-FileHash]()　適用有PowerShell 4.0以上的機器
* [HashTab](http://implbits.com/products/hashtab/)　免費軟體

###其他
* [NegativeScreen](http://arcanesanctum.net/negativescreen/)
* [WinRAR](http://www.rar.com.tw/download.html)　壓縮／解壓縮軟體。雖然是付費軟體，不過過了試用期後還是可以……
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)　虛擬機軟體
* [DAEMON Tools Lite](http://www.disk-tools.com/download/daemon)　虛擬光碟軟體
* [Recuva](https://www.piriform.com/recuva)　檔案救援軟體
* [SetPoint](http://www.logitech.com/zh-tw/mice-pointers/articles/11650)　羅技的鍵盤滑鼠軟體。裝了這個滑鼠的四向滾輪才有做用。
* [Yahoo奇摩即時通](https://hk.messenger.yahoo.com/)　通訊軟體

##疑難雜症
### Vista/Win7的Windows Update抓更新時跑不完，抓不到更新
1. 開啟Windows Update，變更設定為永不檢查更新，變更完後建議重新啟動一次電腦
2. 至Microsoft Security Bulletins下載所有未安裝的安全性更新
3. 手動安裝在2.下載的更新，重新啟動電腦以完成安裝程序
4. 開啟Windows Update，恢復為原本的設定，按`檢查更新`看能否抓到新的更新