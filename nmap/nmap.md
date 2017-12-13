# nmap

nmap的筆記

***

<code>apt-get install nmap</code>
<p>安裝方法

<code>nmap IP</code>
<p>顯示有開通的port、狀態及服務

<code>nmap IP範圍</code>
<p>掃描IP範圍內的主機開通的port、狀態及服務

<code>nmap -sL IP範圍</code>
<p>掃描IP範圍內的主機，其他有-sP,-P0,-PS,-PA,-PU,-PR參數可使用

<code>nmap -T4 IP</code>
<p>列出常用的port、狀態、服務

<code>nmap -v IP</code>
<p>顯示掃描過程

<code>nmap -A IP</code>
<p>顯示所有項目包含作業系統、核心版本、憑證上的標題、服務的版本

<code>nmap -oX - IP > nmap.xml</code>
<p>將結果輸出至nmap.xml

<code>nmap -A -oX - IP > nmap.xml</code>
<p>將所有掃描項目儲存至nmap.xml

<code>nmap -p 範圍(1~65535) IP</code>
<p>掃描範圍內的port

<code>nmap -sS IP</code>
<p>使用TCP SYN掃描其他還有-sT,-sA,-sW,-sM,-sN,-sF,-sX參數可使用

<code>nmap -T3 IP</code>
<p>以預設時序腳本進行掃描其他還有參數T0到T5，數字越小間格越長縮需時間也越長
