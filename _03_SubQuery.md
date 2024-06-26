## **📜 서브쿼리(Sub Query)**
`01. 다수의 쿼리를 결합해 하나의 쿼리로 표현`

`02. ()로 묶어서 하나의 쿼리를 가상의 테이블처럼 활용`

`03. Select, From, Where절에 사용할 수 있음`

---
### 📜 단일행 서브쿼리
`01 서브쿼리의 결과가 하나의 행만 가져오는 쿼리`

`02. 테이블 사용가능`

`03. Where절에서 조건으로도 Select절에서 조회할 컬럼으로도 사용가능`

- ⚠️ 참고
  - 단일연산자(=, !=, >, <, >=, <=...)와 주로 활용
  - 단일연산자 오른쪽에 작성
---
### 📜 다중행 서브쿼리
`01. 서브쿼리의 결과가 여러개의 행을 가져오는 쿼리`

`02. 테이블이나 Where절의 조건으로만 사용가능(In절)`

---
### 📜 다중열 서브쿼리
`01. 서브쿼리의 결과가 여러개의 행과 열을 가져오는 쿼리`

`02. From, Join절에서만 사용가능`

---
### 📜 집합 연산자
`01. 서로 다른 쿼리 결과의 합집합, 교집합, 차집합을 구해주는 함수`

`02. ⚠️ 첫 번째 쿼리에서 컬럼의 개수, 데이터 타입이 결정되기 때문에 두 번째 쿼리는 첫 번재 쿼리의 컬럼의 개수, 데이터 타입을 따라야 함`

#### 01. 합집합
##### 001. UNION
`01. 중복제거 후 합집합 연산`

`02. 각각의 쿼리에서 조회된 결과를 합침`
##### 002.  UNION ALL
`중복제거 없이 각각의 쿼리에서 조회된 결과를 합`

#### 02. 차집합
##### 001. MINUS
`조회쿼리1의 결과에서 조회쿼리2의 결과를 제외한 데이터 조회`
##### 002. EXCEPT
`다른 DB에서는 MINUS 대신 EXCEPT를 사용`
    
#### 03. 교집합
##### 001. INTERSECT
`조회쿼리1의 결과와 조회쿼리2의 결과 중 중복된 데이터만 조회`
  
