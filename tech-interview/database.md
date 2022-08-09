## RDB와 NoSQL의 차이

* #### RDB
관계형 모델을 기반으로 하는 데이터베이스이다.
이를 유지하고 관리하기 위한 시스템이 RDBMS이다.

* 관계형 데이터베이스의 특징
    * 2차원 데이터로 표현된다. (행과 열을 가짐)
    * 관계를 가진 테이블의 집합으로 구성됨
    * 테이블 사이의 관계를 외래키로 나타넴
    * ACID 성질을 갖는다.
    * SQL을 사용해 데이터를 질의한다.

* #### NoSQL
RDB와 달리 테이블 간 관계를 정의하지 않는다.
데이터 테이블은 그냥 하나의 테이블이며 테이블의 관계가 없기때문에 Join이 불가능

* NoSQL의 특징
    * 다양한 방식으로 데이터를 표현한다. (key-value, document 등등)
    * 테이블 사이에 명시된 제약이나 규칙이 없다.
    * 스키마가 고정적이지 않고, 매우 유연하다.
    * 연산이 빠르다.

## 트랜잭션

트랜잭션이란 데이터베이스의 상태를 변화시키기 위해 수행하는 작업의 단위.

상태를 변화시킨다는것은 SQL 질의어를 통해 DB에 접근하는 상황을 일컫는다.

* 작업의 단위란? 

예를 들어 상점에서 한가지의 물품을 사려합니다. 이때 일어나는 쿼리들은
1. 사용자의 계좌에서 물품의 가격만큼 차감하는 쿼리
2. 상품의 재고가 한개 차감하는 쿼리

이렇게 한 작업이 처리되기 까지가 하나의 트랜잭션이다.

트랜잭션의 특징은 바로 ACID이다.

* ACID
    * 원자성 (Actomicity) : 한 트랜잭션 내에서 실행한 적업들은 하나의 단위로 처리한다.
    * 일관성 (Consistency) : 트랜잭션은 일관성 있는 데이터베이스 상태를 유지한다.
    * 독립성 (격리성, Isolation) : 동시에 실행되는 트랜잭션들이 서로 영향을 미치지 않도록 격리해야한다.
    * 지속성 (영속성, Durability) : 트랜잭션을 성공적으로 마치면 결과가 항상 저장되어야 한다.

<br>

* Commit: 트랜잭션이 성공적으로 성공했고 동시에 변경사항들을 저장
* Rollback: 트랜잭션이 비정상적으로 종료되어 트랜잭션의 원자성이 깨진경우 변경사항을 취소

## 트랜잭션 격리 수준
https://martial.tistory.com/2 이건 내가 블로그로 정리했지롱

## Index
추가적인 쓰기 작업과 저장 공간을 활용하여 데이터베이스 테이블의 검색 속도를 향상 시키기 위한 자료구조, 책의 목차와 비슷

## Join

두 개 이상의 테이블을 연결하여 검색하는 방법.
테이블을 연결하기 위해선 최소 한개 이상의 컬럼을 공유하고 있어야 한다.

* 종류
    * Inner Join: 기준 테이블과 join 테이블의 중복된 값을 보여준다.
    * Left Outer Join: 기준 테이블안에서 join 테이블과 중복된 값을 보여준다.
    * Right Outer Join: join 테이블안에서 기준 테이블과 중복된 값을 보여준다.

## Redis

인 메모리 형식의 key-value 데이터 구조를 가진 NoSQL이다. 
Redis는 데이터를 RAM에 저장하기 때문에 속도가 매우 빠르다.

하지만 RAM은 휘발성이기 때문에 
특점 지점을 설정하고 디스크에 백업하는 snapshot이라는 백업 과정이 존재한다.

## Query
쿼리란 데이터베이스에 정보를 요청하는것.

## DDL, DML, DCL

DDL - 데이터베이스의 스키마 객체를 생성, 변경, 제거하거나 권한 부여, 박탈등을 수행하는 문장의 집단이다.
* CREATE
* ALTER
* DROP
* TRUNCATE
* GRANT
등등

DML - 스키마 객체의 데이터를 입력,수정,조회,삭제 등등을 하는 문장의 집단이다.
* INSERT
* UPDATE
* DELETE
* SELECT
등등

DCL - 트랜잭션의 성격을 제어
* SET TRANSACTION
* COMMIT
* ROLLBACK
* SAVEPOINT