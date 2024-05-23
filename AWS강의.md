## 서버 - 20240517
### X-Tier (계층구조)
- 3-Tier (기본)
1. Client Tier  
Web Server, Front-end, Etc.html,js,css
2. Application Tier  
Was Server, Back-end, Etc.class,xml
3. Data Tier  
DB Server, Back-end, ETC.DBMS류  
<br>
### 서버구성도<br>
방화벽->IPS(오류차단)->L4->Web Server->Was Server->백본 스위치2->DB1   
                        (->Web Server->Was Server)           ->DB2  
=>서버 이중화
              
