# spring 카드사 추천 홈페이지 프로젝트

### 프로젝트 기간 : 21.05.06 ~ 21.06.03 

### 프로젝트 수행자 : 이강현

### ec-2 배포 링크 : http://ec2-54-180-39-245.ap-northeast-2.compute.amazonaws.com:8080/
      
###   

## 환경

- Windows 10
- Springboot
- Tomcat 9.0
- MySQL 8.0
- Lombok
- JPA
- JavaScript
- Thymeleaf
- JQuery
- Ajax


## 참고사이트

- 카드 고릴라 (https://www.card-gorilla.com/home)


- 뱅크샐러드 (https://www.banksalad.com/sectors/card)


## 사용 API

1. Oauth2 이용

	* 카카오 로그인 API 
		- https://www.banksalad.com/sectors/card
		
       	* 네이버 로그인 API
       	 	- https://nid.naver.com/user2/campaign/introNaverIdLogin.nhn
		 
       	* 구글 로그인 API		
       		- https://console.cloud.google.com/

## MySQL (RDS) :
	```
	create table board (bbsid bigint not null auto_increment, create_date datetime, modified_date datetime, bbs_category varchar(255) not null, bbs_content varchar(255) not null, bbs_reply varchar(255), bbs_title varchar(255) not null, userid varchar(255), primary key (bbsid)) ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4;



create table card (card_code bigint not null auto_increment, annual_fee integer not null, before_pay integer not null, benefit1 varchar(255) not null, benefit1_detail TEXT, benefit2 varchar(255) not null, benefit2_detail TEXT, benefit3 varchar(255) not null, benefit3_detail TEXT, card_company varchar(255) not null, card_link varchar(255) not null, card_name varchar(255) not null, card_photo TEXT, card_type varchar(255) not null, count integer, primary key (card_code)) ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4;


create table card_company (company_code bigint not null auto_increment, company_logo varchar(255) not null, company_name varchar(255) not null, have_card_num integer not null, primary key (company_code)) ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4;


create table reply (id bigint not null auto_increment, create_date datetime, modified_date datetime, reply_content varchar(300) not null, reply_writer TEXT, bbsid bigint not null, primary key (id)) ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4;


create table user (id bigint not null auto_increment, create_date datetime, modified_date datetime, email varchar(255) not null, name varchar(255) not null, role varchar(255) not null, primary key (id)) ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4;
	
	```

