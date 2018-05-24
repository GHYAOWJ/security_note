# security_note

一些安全性相關筆記

***

|檔名                                    |說明                   |
|----------------------------------------|-----------------------|
|[post get](php/post_get.md)             |post及get的差異        |
|[cookie session](php/cookie_session.md) |cookie及session的差異  |
|[SQL injection](php/sql_injection.md)   |SQL injection原理及防範|
|[網芳漏洞](ms/netbios.md)               |網路芳鄰攻擊及防範     |
|[MS08-067](ms/ms08_067.md)              |ms08-067攻擊及防範     |
|[nmap](nmap/nmap.md)                    |nmap的筆記             |
|[androguard](androguard/)               |androguard apk逆向工程分析 |
|[mobsf](mobsf/)                    |mobsf的筆記 apk靜態及動態分析             |


***

攻擊機:kali linux,目標機:windows xp,metasploitable2,metasploitable3

Nmap,OpenVAS:掃描目標電腦開啟port,服務,漏洞

metasploit:使用search尋找漏洞相關工具

rapid7:進入rapid7的metasploit尋找工具action,options,payload相關設定

***

在metasploit設定相關action,options,payload後執行exploit進行攻擊，視情況需要時使用sseions -i 連線號碼，進入後可執行cli相關指令。

可使用upload,download對目標機進行檔案傳輸。

若目標電腦為windows系列則可使用ps explorer.exe確認explorer.exe的PID執行migrate PID後可使用keyscan_start,keyscan_dump進行鍵盤側錄，screengrab可擷取目標機現在畫面。
