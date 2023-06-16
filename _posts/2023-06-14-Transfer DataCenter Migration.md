Project: 데이터센터 이전에 따른 마이그레이션
---

# 데이터센터 이전에 따른 마이그레이션

+ 기간 : 2023.02 - 2023.06(5개월)
+ 성과 :
    + 데이터센터 이전에 따른 비용 절감
    + 데이터베이스 아키텍쳐 설계 변경(MMM+slave ⇨ MHA)
    + LifeKeeper 시스템 계약 해지를 통한 비용 절감(연간 갱신비용 20,694,000원)
    + 3개의 DB서버 Migration

+ 역할 :
    + 새로운 데이터베이스 아키텍쳐 의견 제시(기존 MMM + Slave구성을 MHA구성으로 변경)
    + 프로젝트 관련팀과 프로젝트 일정 및 작업 방식 조율
    + 3개의 DB서버 구축(MySQL5.6)

+ 획득 역량
    + 데이터베이스 아키텍쳐 및 가용성에 대해 알게되었습니다.
    + 기존 Slave서버를 Master로 승격시 reset slave all, reset master를 통해 기존 Replication 설정에서의 데이터 삭제의 필요성을 배웠습니다.
+ skill :
![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=plastic&logo=mysql&logoColor=ffffff)

+ 작업 일정
  
|날짜|작업 내용|비고|
|------|---|---|
|2023-02|IP, DNS설정, |서버팀에 의뢰|
|2023-02 ~ 03|서버 구축 및 Replication 설정||
|2023-04 ~ 06|Slave서버 승격 작업|한달에 1대씩 실시|
