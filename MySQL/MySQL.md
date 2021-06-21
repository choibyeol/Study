## Mac MySQL 터미널에서 실행하기



1. MySQL이 설치된 곳의 bin 폴더로 이동 -> root 권한으로 MySQL에 접속
2. cd /usr/local/mysql/bin (경로는 환경설정의 MySQL configuration에서 확인 가능)
3. ./mysql -u root -p (-u는 계정, p는 패스워드)
4. 패스워드 입력 후 MySQL 실행



## MySQL 기본 명령어



##### Database 조회

``` mysql
SHOW DATABASES;
```



##### Table 생성

```mysql
CREATE TABLE test;
```

또는 컬럼도 같이 생성(id, name, phone 예시)

```mysql
CREATE TABLE test (
  id int NOT NULL auto_increment primary key,
	name VARCHAR(15) NOT NULL,
	phone VARCHAR(15) NOT NULL
);
```

- INT: 정수형

- DOUBLE: 실수형

- VARCHAR: 문자형

- NOT NULL: 빈 값일 수 없음

- AUTO_INCREMENT: 숫자가 자동으로 증가



##### 생성된 테이블 상세 정보 확인

``` mysql
DESCRIBE test;
```



##### 삽입 (INSERT)



##### 조회 (SELECT)



##### 조건 사용하여 조회



##### 오름차순, 내림차순 정렬 조회



##### 수정 (UPDATE)



##### 전체 삭제

```mysql
DROP TABLE test;
DROP DATABASE testdb;
```







