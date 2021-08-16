# 카드사 추천 홈페이지 프로젝트 (Springboot)

### 프로젝트 기간 : 21.05.06 ~ 21.06.03 

### 프로젝트 수행자 : 이강현

### ec-2 배포 링크 : http://ec2-54-180-39-245.ap-northeast-2.compute.amazonaws.com:8080/
      
### 시연 영상 : https://www.youtube.com/watch?v=iGtQYibdWVs

## 사용 기술 스택

	-개발환경: windows 10 , IntelliJ, MySQL 등.
	
	- Backend: JAVA, Springboot, JPA, MySQL
	
	- Frontent: HTML, CSS, JavaScript, Ajax, JQuerym Thymeleaf
	
	- 기타 : github, AWS
	
	


## 참고사이트

- 카드 고릴라 (https://www.card-gorilla.com/home)


- 뱅크샐러드 (https://www.banksalad.com/sectors/card)






## 참고사항

1. 모든 코드를 MVC패턴에 맞추어 작성.

2. Spring Security를 이용한 보안

3. Oauth2 를 이용한 구글 / 네이버 / 카카오 API 로그인 구현

4. 제품 서비스 외에도, CRUD 게시판 구현

## 데이터베이스
	
	- RDS/ MySQL 이용
		
		*테이블: 회원, 게시판, 게시판_답글(관리자), 카드, 카드사

## 개발 배경

	- 소비자의 상황에 따라, 혜택이 천차만별인 카드를 선별 및 추천 해주는 사이트.
	- 연령별 / 성별/ 혜택별 등의 조건검색, 여러가지 카드 비교, 인기순 카드 차트, 문의 게시판 등이 있음.
	
	
## 홈페이지 구조	
	
 	-로그인 : 카드사에 연결만 해주는 것에 초점을 맞추어 OAUTH2를 이용한 네이버/카카오/구글 로그인으로 구현.
	
	-관리자 : 카드 / 카드사 등록수정삭제, 게시판 답글 등을 구현.
	
	-사용자 : 인기별 카드 차트, 대부분의 페이지에서의 카드별 비교기능, 조건에 따른 검색기능을 구현.
	
# 어려웠던 점 및 해결방법:

프로젝트 중 MVC 패턴이 너무 이해가 안갈 때 Java의 콘솔창만을 이용하여 MVC 스타일의 게시판 구현을 병행해봄.

https://github.com/lkh599810/Console_Java

	
+콘솔창 게시판으로는 약간의 부족함이 있어 JavaFX를 이용한 MVC패턴의 게시판도 구현.

https://github.com/lkh599810/FX_MVC
