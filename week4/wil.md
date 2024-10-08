### 데이터베이스
- 데이터베이스(Database)는 체계적으로 데이터를 저장하고 관리하는 시스템
- 데이터를 효율적으로 저장, 검색, 수정, 삭제할 수 있도록 설계된 구조
- 다양한 애플리케이션에서 데이터를 저장, 관리
- 데이터를 쉽게 접근하고 분석할 수 있도록 도와줌

#### 관계형 데이터베이스 (RDBMS: Relational Database Management System)
- 데이터를 행(Row)과 열(Column)로 구성된 테이블(Table) 형태로 저장하는 데이터베이스
- 테이블 간에 관계를 정의하고, 이를 통해 데이터를 연결하고 조작
  - 예시: MySQL, PostgreSQL, Oracle, Microsoft SQL Server
##### 특징
- SQL을 사용하여 데이터 관리
- 데이터의 일관성과 무결성을 유지하기 위한 제약 조건 사용
- ACID 특성을 지원: 원자성, 일관성, 고립성, 내구성
#### 비관계형(NoSQL) 데이터베이스
- 테이블을 사용하지 않고 데이터를 저장하는 방식
- 스키마가 고정되지 않아 유연하게 데이터를 저장할 수 있음
  - 예시: MongoDB, Cassandra, Redis, Couchbase
#### 객체 지향 데이터베이스 (OODBMS: Object-Oriented Database Management System)
- 객체 지향 프로그래밍에서 사용하는 객체(클래스, 상속, 다형성)를 데이터베이스로 사용
  - 예시: db4o, ObjectDB
#### 임베디드 데이터베이스 (Embedded Databases)
- 애플리케이션 내부에 내장된 데이터베이스
- 실행될 때 함께 실행되는 데이터베이스

### 장고 Model
- Model은 데이터베이스의 테이블과 대응
- 테이블의 열(Column)은 장고 모델에서 필드(Field)로 정의
- 모델은 클래스로 정의
- 각 클래스는 데이터베이스의 하나의 테이블
- 클래스의 속성들은 데이터베이스의 테이블에서 열에 해당
#### 사용
- 모델을 정의하려면 models.py 파일에 클래스를 정의
- django.db.models.Model을 상속
- 모델을 정의한 후, 해당 모델을 데이터베이스에 반영하기 위해 마이그레이션
