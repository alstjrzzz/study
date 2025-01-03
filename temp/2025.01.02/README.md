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

REST API에서 서버는 요청에 대한 명확한 응답을 제공하여야 함(200 ok, 404 not found , ...)

백엔드에서 db 사용하는 프레임워크는 jpa, mybatis

db 접속 편하게 하려고 sql mapper, orm(object relational mapping) 둘 중에 하나

### sql mapper

내가 작성한 sql 결과(반환받은 db데이터)을 자바 객체에 매핑

mybatis

#### 장점

1. 수동 작성이라 고성능 쿼리 작성 가능
2. 복잡한 쿼리 처리 굿

#### 단점

1. sql 작성 많아지면 코드 관리 ㅈ
2. 유지보수할때 매핑 동기화 문제 발생 가능

### orm

db데이터를 자동으로 매핑

jpa/hibernate

#### 장점

1. 쿼리 자동 생성이라 코드 간결
2. db변경 용이
3. 객체지향적 코딩 ㄱㄴ

#### 단점

1. 쿼리 비효율적일수도
2. 복잡한 쿼리 한계있음
3. 공부해야됨ㅋ


전세계적 jpa 우세

한국 중국만 mybatis 많이 씀

lombok의 @Data: getter, setter, 생성자 등등 자동 생성

mybatis에서 @Mapper로 MapperInterface 만들고 mapper.xml에 sql작성



로그인하면 그 유저의 닉네임과 todos를 보내야할건데...
