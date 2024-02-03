# 📋 JSP 게시판

### 프로젝트 소개

- JSP, AWS EC2를 사용하여 게시판 구현 및 배포
- 주소 : http://13.209.67.168:8080/ListTest_newLecture/views/main.jsp

## 
   - ### JSP을 이용하여 게시판 구현을 하였습니다.
   - ### 일반 로그인
     ![registerAndLogin](https://github.com/oidolee/jsp_board2/assets/85022962/b2039528-bf04-48f7-9488-7749fb123158)




   - ### 관리자 로그인 ( 관리자로 로그인시 모든 수정, 삭제 권한 부여)
      ![admiin](https://github.com/oidolee/jsp_board/assets/85022962/b84552e3-e1f3-494d-8e96-34db30141c8b)


## 1. 개발 환경

- Front : HTML, Bootstrap
- Back-end : JSP
- 버전 및 이슈관리 : Github
- 서비스 배포 환경 : AWS EC2
<br>


## 2. 프로젝트 구조

```
..(jsp project)
    └── src
        └── main
            ├── java
            │       ├── list
            │       │    ├── List.class
            │       │    └── ListDAO.class    
            │       │ 
            │       ├── post
            │       │    └── DBConn.class
            │       │ 
            │       └── user
            │            ├── User.class
            │            └── UserDAO.class
            │
            └── webapp
                  └── Globalstyled.jsx
                         ├── controller
                         │    ├── listDeleteController.jsp
                         │    ├── listInsertController.jsp
                         │    ├── listUpdateController.jsp
                         │    ├── loginController.jsp
                         │    ├── logOutController.jsp
                         │    └── registerController.jsp
                         ├── css
                         │    └── common.css
                         ├── dist
                         │    ├── css
                         │    │    ├── bootstrap.min.css
                         │    │    └── bootstrap.min.css.map
                         │    └── js
                         │         ├── bootstrap.bundle.min.js
                         │         └── bootstrap.bundle.min.js.map
                         ├── META-INF
                         │    └── MANIFEST.MF
                         ├── views
                         │    ├── header.jsp
                         │    ├── list.jsp
                         │    ├── listInsert.jsp
                         │    ├── listUpdate.jsp
                         │    ├── login.jsp
                         │    ├── main.jsp
                         │    └──register.jsp         
                         ├── views
                         │    ├── header.jsp
                         │    ├── list.jsp
                         │    ├── listInsert.jsp
                         │    ├── listUpdate.jsp
                         │    ├── login.jsp
                         │    ├── main.jsp
                         │    └──register.jsp     
                         ├── WEB-INF
                         │    └── lib
                         │          └── web.xml
                         ├── form.html
                         ├── index.jsp
                         └── login.html

```

## 3. 주요 코드 설명

   - ### UserDAO
      ![image](https://github.com/oidolee/jsp_board/assets/85022962/0995f43f-cbac-4081-878f-5363c1c000d5)
     <br> 
   - ### UserDAOIpl.java
     ![image](https://github.com/oidolee/jsp_board/assets/85022962/7b89ba1c-6d16-4dfe-97d3-9702cc657d2f)

   - ### ListDAO
     ![image](https://github.com/oidolee/jsp_board/assets/85022962/88978738-dbbc-46ce-87c4-eca44f5ca81e)

   - ### ListDAOIpl
     ![image](https://github.com/oidolee/jsp_board/assets/85022962/9b9e67a1-a425-4122-b9ef-33ed7122901b)

     
   - ### registerController.jsp (userBean 통해 회원가입 등록데이터 입력)
      ![image](https://github.com/oidolee/jsp_board/assets/85022962/697ea560-d4fb-4960-b28b-1f54e3f8fde3)



## 3. DB
   - ### MySQL 사용
      - ### ERD
        ![image](https://github.com/oidolee/jsp_board/assets/85022962/5db1ed8d-4fd5-45f9-9c1d-5bafdb71d625)

      - ### 테이블
        ![image](https://github.com/oidolee/jsp_board/assets/85022962/90ca9d52-9191-4e0d-9048-d57b0b781dd2)


## 4. 느낀점
   - JSP를 처음 써보면서 기존 PHP와 비슷한점이 있어 쉽게 접근 할 수 있었습니다.
   - DB 연결 및 AWS EC2를 이용하여 배포 한 부분에서 조금 어려웠지만 해당 과정을 알 수 있었습니다.


