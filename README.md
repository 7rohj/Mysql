# Mysql

1. 칼럼명은 영어로 지원 
2. 내용에 한글 있으면 에러뜸
3. 해결 : </br>

`테이블 만들때` 

```
CREATE TABLE [테이블명] (
[컬럼명] [데이터타입] (NOT NULL / DEFAULT NULL), 
PRIMARY KEY([기본키로 지정할 컬럼명])
) ENGINE=[엔진명] DEFAULT CHARSET=[인코딩]
```

`만들어져 있는 경우`

```
alter table [테이블명] engine=[엔진];
alter table [테이블명] DEFAULT CHARACTER SET [문자셋];
alter table [테이블명] engine=[엔진], DEFAULT CHARACTER SET [문자셋];
```

(추가 : ENGINE=InnoDB DEFAULT CHARSET=utf8 )
