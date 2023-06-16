Project: 물리서버 가상화 Migration
---
# "물리서버 가상화"

+ 기간 : 2022.11.01 - 2023.02.27(3개월)
+ 성과 :
  + 데이터베이스센터 이전에 따른 비용 절감
  + 2개의 물리서버 가상화 
+ 역할 :
    + Mysqldump, Restore 및 Replication을 이용한 slave MySQL5.6 DB서버 구축
        + 백업용 slave서버 2개, 부하분산용 slave서버 2개
    + Jenkins를 이용한 물리서버와 가상서버의 퍼포먼스 차이 조사
    + 프로젝트 관련팀과 프로젝트 일정 및 작업 방식 조율
+ 획득 역량 :
    + mysqldump, restore 및 replication을 이용한 DB서버 구축방법을 익혔습니다.
    + 물리서버와 가상서버의 퍼포먼스 차이를 직접 조사해 둘의 차이를 알게되었습니다. 
  
+ skill :
  ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=plastic&logo=mysql&logoColor=ffffff)
  ![jenkins](https://img.shields.io/badge/-jenkins-D24939?style=plastic&logo=jenkins&logoColor=ffffff)
+ 작업 일정
  
|날짜|작업 내용|비고|
|------|---|---|
|2022-11|IP, DNS설정|서버팀에 의뢰|
|2022-12|서버 구축 및 Replication 설정||
|2023-01 ~ 02|서버 이전|load balancer작업 실시|
|2023-02|서버 폐기||


+ 작업 방식
    + 부하분산용 서버 이전 - 부하 분산용 서버를 참조하고 있는 개발측 batch가 있었다.
    + load balancer에 s04추가 ⇨ 상황 대기(1주일) ⇨ load balancer에서 s01 제거
    + load balancer에 s05추가 ⇨ 상황 대기(1주일) ⇨ load balancer에서 s02 제거
    + 참고 : s04,s05는 새로운 부하 분산용 slave 서버 s01,s02는 기존 부하 분산용 slave 서버
