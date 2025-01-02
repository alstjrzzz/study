# todo-list project

## 사용기술

spring boot, rest api, mybatis, 배고파

### rest api란 뭘까나

**RE**presentational **S**tate **T**ransfer **API**

서버-클라이언트 간 통신을 위한 아키텍쳐 스타일 

1. http uri로 리소스를 정의하고
2. http method로 리소스의 행위 정의

#### http uri(uniform resource identifier)

규칙

1. 명사 사용
2. /로 계층 관계
3. 소문자 작성


#### http method

|메서드|목적|
|:---:|:---:|
|POST|조회|
|GET|생성|
|PUT|전체 수정|
|PATCH|일부 수정|
|DELETE|삭제|

## spring initializr 종속성 추가

lombok, spring web, spring security, mysql driver, mybatis framework

## 프로젝트 기능

로그인, 회원가입, 리스트 추가, 삭제


테이블: users, todos

rest api

POST/auth/signup
POST/auth/login
GET/todos/{id}
POST/todos/{id}


dto(data transfer object): 데이터를 전달하는 용도의 객체 
