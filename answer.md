1. 관계형 데이터베이스(RDBMS)와 비관계형 데이터베이스(NoSQL)의 장단점 비교

- 관계형 데이터베이스 장점
  - Data를 Column과 Low 형태로 저장한다.
  - 데이터의 분류, 정렬, 탐색 속도가 빠르다.
  - 정규화를 통해 중복 데이터를 최소화할 수 있다.
- 관계형 데이터베이스의 단점
  - 반드시 스키마 규격에 맞춰서 데이터를 다뤄야한다.
  - 데이터 처리에 대한 부하 발생시 처리가 어렵다.
 
- NoSQL의 장점
  - 데이터간의 관계를 정의하지 않아도 된다.
  - RDBMS보다 복잡도가 떨어져, 훨씬 대용량의 데이터를 저장, 관리 할 수 있다.
- NoSQL의 단점
  - key값에 대한 입,출력만 지원한다.
  - 스키마가 정해져 있지 않아, 데이터에 대한 규격화가 되어있지 않다.
  - 중복 데이터가 존재해 탐색의 성능이 느리다.

2. 트랜잭션(transaction)이란 무엇인가요?

- 트랜잭션이란 데이터베이스 시스템에서 하나의 논리적 기능을 정상적으로 수행하기 위한 작업의 기본 단위를 말한다. </br>SQL를 통해 데이터베이스에 접근하는 것을 의미(SQL : SELECT, INSERT, DELETE, UPDATE..) </br>트랜잭션이 안전하게 수행되기 위해서는 ACID를 만족해야한다.

3. MySQL에서 조인(join)의 역할은 무엇인가요? 다양한 join의 방식에 대해 설명해주세요.

- 조인이란 두 개 이상의 테이블이나 데이터베이스를 연결하여 데이터를 검색하는 방법이다.
- 조인의 종류
  - INNER JOIN : 교집합으로, 기준 테이블과 조인 테이블의 종복된 값을 보여준다.
  - LEFT OUTER JOIN : 기준 테이블값과 공통으로 존재하는 데이터를 보여준다.
  - RIGHT OUTER JOIN : 조인 테이블값과 공통으로 존재하는 데이터를 보여준다.
  - FULL OUTER JOIN : 합집합으로, 기준 테이블과 조인 테이블의 모든 데이터를 보여준다.
  - CROSS JOIN : 모든 경우의 수를 보여준다.
  - SELF JOIN : 자기자신과 자기자신을 조인하는 것이다. 하나의 테이블을 여러번 복사해서 조인한다고 생각하면 편하다.

4. MySQL에서 인덱스(index)란 무엇인가요?

- 인덱스란 데이터를 빠르게 찾을 수 있는 수단으로서, 테이블에 대한 조회 속도를 높여주는 자료 구조이다. </br> 인덱스는 테이블의 특정 레코드 위치를 알려주는 용도로 사용한다. </br>색의 색인을 떠올리면 쉽다.
