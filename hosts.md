# Hosts

透過 hosts 設定檔可手動設定主機名稱與 IP 位址 。     
通常網路上公開的網站都是透過 DNS 伺服器來查詢網址與 IP 的對應關係，不會使用 hosts 設定檔，會寫在 hosts 檔中的大部分都是內部網路的主機，也就是私人的主機。     
網站的管理者也時常使用 hosts 設定檔來測試自己網站 。

####Windows 系統
hosts 設定檔路徑是：C:\WINDOWS\system32\drivers\etc\hosts 。     
hosts 設定檔沒有任何副檔名，所以在開啟時要自行選擇編輯器，可以用記事本開啟 (點選記事本，按右鍵，點選＂以系統管理員身分執行＂，開啟host設定檔，以系統管理員身分進行更改檔案後才可以存檔成功。    
hosts 設定檔的內容預設應該都只有註解（# 開頭的就是註解），我們可以在檔案的最後加上自己的設定，第一個欄位是 IP 位址，然後使用空白或 Tab 分隔，第二個欄位就放主機的 FQDN（也就是網址）。    
範例:  102.54.94.97     rhino.acme.com 

####Linux 系統
hosts 設定檔放在/etc/hosts。    
如果要修改它，要使用 root 管理者權限修改：sudo vi /etc/hosts。




![Host檔設定](https://blog.gtwang.org/wp-content/uploads/2016/04/windows-hosts-file-configuration-8.png)

---
> 參考網址
- 手動設定網址與IP對應的Hosts檔 <https://blog.gtwang.org/windows/windows-linux-hosts-file-configuration/>
- DNS <http://dns-learning.twnic.net.tw/dns/01whatDNS.html>
