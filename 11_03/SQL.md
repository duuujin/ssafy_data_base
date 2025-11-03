# SQL
- Structure Query Language
- 테이블의 형태로 구조화 된 관계형 데이터베이스에게 요청을 질의요청

# SQL Statements
- SQL을 구성하는 가장 기본적인 코드 블록

# SQL Statements 4가지 유형
1. DDL - 데이터 정의
    - 데이터의 기본 구조 및 형식 변경
        1. CREATE
        2. DROP
        3. ALTER
2. DQL - 데이터 검색
    - 데이터 검색
        1. SELECTE
3. DML - 데이터 조작
    - 추가, 수정, 삭제
        1. INSERT
        2. UPDATE
        3. DELETE
4. DCL - 데이터 제어
    - 데이터 및 작업에 대한 사용자 권한 제어
        1. COMMIT
        2. ROLLBACK
        3. GRANT
        4. REVOKE

# Sorting data
## ORDER BY
- FROM clause 뒤에 위치
- 하나 이상의 컬럼을 기준으로 결과를 오름차순(ASC, 기본 값), 내림차순(DESC)으로 정렬
- 예시(오름차순)
    ```SQL
    SELECT
        FirstName
    FROM
        employees
    ORDER BY
        FirstName;
    ```
- 예시(내림차순)
    ```SQL
    SELECT
        FirstName
    FROM
        employees
    ORDER BY
        FirstName DESC;
    ```
- 테이블 customers에서 Country 필드를 기준으로 내림차순 정렬한 다음 City 필드 기준으로 오름차순 정렬하여 조회
- 예시
    ```SQL
    SELECT
        Country, City
    FROM
        customers
    ORDER BY
        Country DESC, City;
    ```
- 정렬에서의 NULL
    - NULL 값이 존재할 경우 오름차순 정렬 시 결과에 NULL이 먼저 출력
- SELECT statement 실행 순서
    1. FROM
    2. SELECT
    3. ORDER BY
