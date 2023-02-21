# SQL_study
 1. 기본적인 흐름
 2. 문자열
		 2.1  SUBSTR
		 2.2 REPLACE
 3. 숫자
		 3.1 ROUND
		 3.2 AVG
		 3.3 SUM
 4. 날짜
		 4.1 DATE_FORMAT
 5. 조건
		 5.1 IS NOT
		 5.2 ORDER BY
		 5.3 IFNULL
		 5.4 WHERE
		 5.5 GROUP BY
		 5.6 HAVING
 6. JOIN
		 6.1 INNER JOIN

기본적인 흐름|&nbsp;
:---|:---
SELECT *| 
FROM [TABLE1] AS A|
&nbsp;&nbsp;&nbsp;&nbsp; JOIN [TABLE2] AS B|
&nbsp;&nbsp;&nbsp;&nbsp; ON A.column1 = B.column2|
WHERE 조건|
GROUP BY A.column1|
HAVING 조건|
|
<br>

-------------------------------------------------------

문자열|&nbsp;|&nbsp;
:---|:---|:---:
문법|설명|비고 
SUBSTR(column, location, n)|문자열 column을 location(위치, 첫번째는 1)부터 n개 잘라냄|
REPLACE(column, "A", "B")|문자열 column의 "A"를 "B"로 |
<br>

숫자|&nbsp;|&nbsp;
:---|:---|:---:
문법|설명|비고 
ROUND(column, 반올림자리) | 기본자리값 0(소수 첫째자리) <br> 음수면 소수, 양수면 정수 방향으로 자리 이동
AVG(column) | 평균 |
SUM(comumn) | 합계 |
<br>

날짜|&nbsp;|&nbsp;
:---|:---|:---:
문법|설명|비고 
DATE_FORMAT(column, format) | 날짜 형식(으로) 변환 | "%Y-%m-%d"
<br>

조건|&nbsp;|&nbsp;
:---|:---|:---:
문법|설명|비고 
IS NOT | 조건에 해당하지 않는 | !=    
ORDER BY | 정렬 | 기본 오름차순(ASC) <br>내림차순은 DESC                       
IFNULL(column, A) | if( column == null): <br> &nbsp;&nbsp;&nbsp;&nbsp; return column <br> else : <br> &nbsp;&nbsp;&nbsp;&nbsp; return A 
WHERE | select할 column에 조건을 준다.
GROUP BY | column을 기준으로 group by 하여 group by 기준으로 AVG, SUM 등등 적용
HAVIGN | GROUP BY를 적용한 후 조건 | 이때 WHERE를 쓰면 에러
<br>

JOIN|&nbsp;|&nbsp;
:---|:---|:---:
문법|설명|비고 
FROM [TABLE1]  <br> &nbsp;&nbsp;&nbsp;&nbsp; (INNER)JOIN [TABLE2] <br> &nbsp;&nbsp;&nbsp;&nbsp; ON [TABLE1].column1 = [TABLE2] | INNER JOIN | 
