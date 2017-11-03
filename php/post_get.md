# post_get

post及get的差異

***

*	POST及GET是在HTML傳送表單資料的方法
*	使用Wireshark擷取傳送過程可發現HTML Form URL Encoded application/x-www-form-urlencoded中顯示POST傳送的資料，而Request URI Query Paramter顯示使用GET傳送的資料
*	在預防資料被擷取可使用https，https是將http的傳送過程中透過SSL/TLS加密封包，https的使用方法首先透過openssl建立crt及key，啟動apache的SSL模組後進入conf將建立的crt及key路徑補上即可
*	get會將傳送的資料參數帶在網址上做請求，雖然透過https可使傳送資料的過程加密，不過依然會在client端的歷史瀏覽或web server端的log留下網址請求紀錄，使用個人資料或者密碼傳送時選擇get較不安全
