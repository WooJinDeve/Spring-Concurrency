## 🍃 스프링 시큐리티 기본 로그인


### 개요
- [[Inflearn]재고시스템으로 알아보는 동시성이슈 해결방법](https://www.inflearn.com/course/동시성이슈-재고시스템?inst=3651d991&utm_source=instructor&utm_medium=referral&utm_campaign=inflearn_트래픽_promotion-link)를 수강후 정리한 레퍼지토리입니다.

### 기본 설정
- **스프링 시작**
    - [https://start.spring.io/](https://start.spring.io/)

- **Spring Package Setting**
    - `Java Version` : 11
    - `Project` : `Gradle Project`
    - `Packaging`
        - `Spring Boot` : `Jar`
    - `Dependencies`
        - `Spring Web`, `Spring DATA JPA`, `MySQL Driver`, `Spring Data Redis`

### Issues
- [[#1] Docker Run port Error](https://github.com/WooJinDeve/Spring-Concurrency/issues/1#issue-1380281276)

### 도커 기본 설정

```
//MySql 이미지 생성
docker pull mysql
docker run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=1234 --name mysql mysql

//MYSQL 데이터 베이스 생성
create database stock_example;

//Redis 이미지 생성
docker pull redis
docker run --name myredis -d -p 6379:6379 redis
```