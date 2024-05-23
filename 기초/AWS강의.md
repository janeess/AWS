## 서버 - 20240517
### X-Tier (계층구조) *
- 3-Tier (기본)
1. Client Tier  
Web Server, Front-end, Etc.html,js,css
2. Application Tier  
Was Server, Back-end, Etc.class,xml
3. Data Tier  
DB Server, Back-end, ETC.DBMS류  
### 서버구성도  <br>    
방화벽->IPS(오류차단)->L4->Web Server->Was Server->백본 스위치2->DB1   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(->Web Server->Was Server)&nbsp;&nbsp;->DB2  
=>서버 이중화 
#### L4  
4계층의 스위치, 서버 살아있는지 health 체크 역할(즉, 정상 서버에만 requeset 토스)  
서버 toss 방법 = Hash, Round
#### 이중화 목적 *
1. High Available(HA) : 고 가용성(1번 서버가 죽어도 2번서버가 돌아가기 때문)  
2. Load Balancing(LB) : 트래픽 분산
### 서버 종류
 - Web Server   
Apache, WebToB, Iboss EWS, Nginx
 - Was Server   
Tomcat, Jboss EAP(Wildfly), Jeus, Weblogig,SebSphere
 - OS Server   
Red Hat, CentOS, Fedora Oracle, Ubuntu  
### 클라우드, 가상화 서버
가상화 서버 = 예를 들어 서버 4개를 한개로 묶어서 만들어진 큰 서버
클라우드 = 묶여진 가상화 서버 수만개를 묶으면 클라우드!
### 클라우드 종류
1. 프레미스 : Data, Application, Server, OS, H/W
2. Iaas :  Data, Application, Server, OS (처음부터 구축)
3. Paas :  Data, Application ( 틀은 있고, 그 이후부터 구축 - 서버 필요 x, 어플리케이션만 구축)
4. Saas :  Data (전부 다 구축되어있음 - 데이터만 관리 ex) mail 서비스)
### 범위
클라우드 - 가상화서버 - 사설 - 범용
### 스케일링
서버 up,down,in,out  
스케일링 up : 기능이 올라갈 때 
스케일링 down : 기능이 내려갈 때  
스케일링 out : 불안정할 시 VM을 자동으로 생성할 때
스케일링 in : 자동 생성된 VM이 다시 줄어들 때 (안정화 될 때)















