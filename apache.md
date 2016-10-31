# Apache

Apache的基本設置主要交由httpd.conf來設定管理，要修改Apache的相關設定，主要是透過修改httpd.cong來實現，修改內容儲存後，需Apache Restart。httpd.conf的內容，主要分成3大部分：

1.  Global Environment （即全局環境變數）
2.  'Main' server configurationphpma.com (定義主要或者預設服務參數的指令，也為所有虛擬主機提供預設的設定參數)
3.  Virtual Hosts (虛擬主機的設定參數)

檔案路徑為AppServ\Apache24\conf\httpd.conf (使用編輯軟體開啟)

|Line|指令|說明|
| ------| ------ |------ |
|60  | Listen 3000/Listen 12.34.56.78:80  |使用其它的連接端口或IP |
|228 | ServerAdmin admin@example.com　    |管理員的電子郵件地址         |
|237 | ServerName localhost:80　　　　    | 指定Apache用於識別自身的名字和埠號。此為主機名稱，如果沒有域名，也可以用IP |
|261 | DocumentRoot "usr/local/httpd/htdocs"  |此目錄為apache放置網頁的地方，裡面的index.html即為連到此主機的預設首頁|
|262 | Directory "C:/AppServ/www"             | 此目錄設定用戶放置網頁的目錄（public_html）的執行動作。   |
|276 | Options Indexes FollowSymLinks | 讓你的Link能連接到其他目錄。 |
|277 | Options None |？  |
|284 | AllowOverride All | ？ |
|297 | irectoryIndex index.html index.htm index.php   | 這裡設定預設主頁的名稱，會自動找到此檔案 |
|515 |Virtual hosts |虛擬主機|
|516 |Include conf/extra/httpd-vhosts.conf|用記事本打開此檔編輯|


---
>參考網址:
- httpd.conf主要設定 <http://www.twisu.com.tw/5/linset/www1.htm>
- Apache 的 httpd.conf 文件設定參數詳解 <http://inspiregate.com/internet/host-setting/79-apachea39s-httpdconf-file-to-set-arguments-detailed.html
-  Apacheh的http.conf中文說明 <http://idobest.pixnet.net/blog/post/22040519-%5B%E8%BD%89%E8%B2%BC%5Dapache%E7%9A%84httpd.conf%E4%B8%AD%E6%96%87%E8%AA%AA%E6%98%8E>
