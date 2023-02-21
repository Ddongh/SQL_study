# SQL_stydy
### 공통

● IFNULL(column, A) : column의 값이 NULL 이 아니면 기존의 data, NULL이면 A로 변경 

### 문자

● SUBSTR(column, location, n) : 문자열 column을 location(위치, 첫번째는 1)부터 n개 잘라냄

● REPLACE(column, "A", "B") : 문자열 column의 "A"를 "B"로 

### 숫자

● ROUND(column, 반올림자리) : 기본자리값 0(소수 첫째자리)
                           음수면 소수, 양수면 정수 방향으로 자리 이동
                         
● AVG(column) : 평균

● SUM(comumn) : 합계


### 날짜

● DATE_FORMAT(column, format) : 날짜 형식(으로) 변환 
                              ex) "%Y-%m-%d

### 조건(WHERE)

● IS NOT : 조건에 해당하지 않는 
         !=
         
● ORDER BY : 정렬
           기본 오름차순(ASC) 
           내림차순은 DESC

### JOIN

● FROM [TABLE1] AS A           : TABLE1과 TABLE2를 INNER JOIN
    INNER JOIN [TABLE2] AS B     primary key -> A.column = B.column
    ON A.column = B.column
    
### GROUP BY

● GROUP BY column : column을 기준으로 group by
                    이후 group by 기준으로 AVG, SUM 등등 
