# Http Protocal

HTTP 狀態碼指的是從伺服器端回應(HTTP Response)的狀態，對於狀態的分類可區分三個層級，分別用三個數字表示，第一個數字為大類、第二個數字為中類、第三個數字為小類。    
完整的狀態碼定義可以參考 RFC 2616 Hypertext Transfer Protocol -- HTTP/1.1 的 10 Status Code Definitions 章節，裡面有完整且詳盡的說明。
不過在 IIS 中有不少微軟自訂的擴充狀態碼，格式類似 404.0 這樣，清楚的狀態碼對於除錯很有幫助。     
HTTP 狀態碼大致分成 5 類 (粗體表示)。
常用的狀態碼如下:

* 200 - 確定。 用戶端要求成功。
* 301 - 要求的網頁已經永久改變網址。此狀態要求用戶端未來在連結此網址時應該導向至指定的 URI。
* 302 - 物件已移動，並告知移動過去的網址。
* 401 - 拒絕存取。
* 403 - 禁止使用。
* 404 - 找不到。
* 500 - 內部伺服器錯誤。
* 504 - 閘道逾時。

---
>參考網址
- HTTP狀態碼 <http://blog.miniasp.com/post/2009/01/16/Web-developer-should-know-about-HTTP-Status-Code.aspx>
