# sql_injection

SQL injection原理及防範

***

SQL injection是一種在input輸入參數時並帶上額外SQL指令，使資料庫執行語法時亦會執行額外的SQL指令的攻擊

例如在登入時帶上' or 1='1'就算密碼不正確依然會有回傳結果使其能登入，在更新或刪除資料時輸入上述判斷則會導致所有資料被修改或刪除

php上SQL injection的預防可透過PDO的bindValue或mysqli的bind_param進行參數化查詢，或者透過Laravel或Codeigniter等framework，使用framework提供的資料庫語法進行操作
