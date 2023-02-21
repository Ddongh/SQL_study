# SQL_stydy

● ROUND(column, 반올림자리) : 기본자리값 0(소수 첫째자리)
                           음수면 소수, 양수면 정수 방향으로 자리 이동
                         
● AVG(column) : 평균

● SUM(comumn) : 합계

● DATE_FORMAT(column, format) : 날짜 형식(으로) 변환 
                              ex) "%Y-%m-%d
                              
● IS NOT : 조건에 해당하지 않는 
         !=
         
● ORDER BY : 정렬
           기본 오름차순(ASC) 
           내림차순은 DESC

● FROM [TABLE1] AS A           : TABLE1과 TABLE2를 INNER JOIN
    INNER JOIN [TABLE2] AS B     primary key -> A.column = B.column
    ON A.column = B.column
