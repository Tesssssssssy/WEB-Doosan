# WEB SW Studio and Talent Donation
Web programming team project for 'Doosan enerability' which is developed by 임태우, 이은주, 박규현



## 프레임워크 및 라이브러리
- Python Flask (Flask, SQLAlchemy, flask_login, werkzeug.security, wtforms etc)
- html/css
- javascript
- Bootstrap
- sqlite3 (db)

## 설치 방법
- git clone https://github.com/Tesssssssssy/WEB-Doosan.git
- python-flask 가상환경 설치 (pip install virtualenv)
- flask_login, sqlalchemy 등 필요한 라이브러리 설치
- python interpreter 변경 후 anaconda를 이용한 flask run


## 웹 기능 

### 회원가입

<img width="1552" alt="register" src="https://user-images.githubusercontent.com/112614954/208710680-0d34fa2e-7996-4e12-8c34-312c8f510cf9.png">

회원가입 페이지에서 사용자의 직급을 선택하여 관리자에게 권한을 부여하여 작업자는 접근할 수 없는 관리자만이 접근할 수 있는 페이지를 따로 구현했습니다.
작업자에게 navbar에서 보이지 않을 뿐더러 라우팅으로 '/' 접근 시도해도 접근할 수 없습니다.

### 로그인

<img width="1552" alt="login" src="https://user-images.githubusercontent.com/112614954/208709567-125db37d-d248-4e5f-b4d4-cc2b3bf60d42.png">


### 홈화면

<img width="1552" alt="index" src="https://user-images.githubusercontent.com/112614954/208709811-202ad13a-b26d-4d3d-a7ed-e7ee18c177b1.png">

홈 화면에서 오늘의 컨디션 정보를 선택하고 제출하면 sqlite3 database에 저장됩니다. 

<img width="612" alt="index(반응형" src="https://user-images.githubusercontent.com/112614954/208709828-5fbb8715-6140-4c26-be3e-1c6becd32a31.png">

css 미디어 쿼리를 통해 사용하는 기기의 사이즈에 맞춰 볼 수 있는 반응형 웹을 구현했습니다. 

### 마이페이지

<img width="612" alt="mypage(반응형 웹" src="https://user-images.githubusercontent.com/112614954/208710206-6f165466-5416-49e5-8bd3-63e1e1c0b551.png">

회원가입 시 입력한 개인정보를 마이페이지에서 확인 및 수정할 수 있습니다. (직급, 성명, 이메일은 변경할 수 없습니다. )

### 게시판 
#### 1. 게시글 목록
![KakaoTalk_Photo_2022-12-21-12-34-10 001](https://user-images.githubusercontent.com/112614954/208814868-ce4a224e-5050-44d9-9546-5fd98edfa8d8.jpeg)

게시판에 등록된 글 목록을 card를 이용해 구현했습니다. 

#### 2.게시글 등록 
<img width="1552" alt="게시글 작성" src="https://user-images.githubusercontent.com/112614954/208822817-be8e5a44-0bb4-4886-86bf-0a776d16df5b.png">


게시판에 올릴 글을 쓰는 페이지입니다. 



#### 3. 게시글 보기 

<img width="1552" alt="게시글 보기 " src="https://user-images.githubusercontent.com/112614954/208823486-1bb93a77-fe0e-4812-b883-b8fe5bfbdbfa.png">

<img width="1552" alt="댓글작성" src="https://user-images.githubusercontent.com/112614954/208821947-5a8b6d68-6ec7-4da4-92fe-aa442a7690c5.png">

 css 미디어쿼리를 통해 만든 웹 반응형 게시글입니다. 게시글에서 수정과 삭제를 할 수 있으며 댓글 기능을 구현했습니다. 댓글은 삭제만 가능합니다. 
 

#### 4. 게시글 삭제 및 수정 기능
<img width="1552" alt="게시글 수정" src="https://user-images.githubusercontent.com/112614954/208821907-f935a2d5-e04a-48d5-a855-1b79e8803c28.png">

삭제/수정 버튼을 통해 글을 삭제 및 수정할 수 있습니다. 


### 관리자 페이지 
![KakaoTalk_Photo_2022-12-21-12-34-10 003](https://user-images.githubusercontent.com/112614954/208816550-2f52fdb1-32b5-4310-84af-592fe8fd15a4.jpeg)

<img width="1058" alt="admin" src="https://user-images.githubusercontent.com/112614954/208816495-59945185-ef70-4cb3-af60-4d9d29a4605b.png">

사용자들이 입력한 정보를 관리자가 볼 수 있도록 정리하여 만든 페이지입니다. 

<img width="943" alt="admin page 1" src="https://user-images.githubusercontent.com/105422037/208861967-b4bcb765-888d-49c7-8f82-4f788776b388.png">

<img width="749" alt="admin page 2" src="https://user-images.githubusercontent.com/105422037/208862529-ac68215f-d4b1-4703-8d7e-0e6c13f7b3b2.png">

<img width="643" alt="admin page 3" src="https://user-images.githubusercontent.com/105422037/208862623-28df20f1-8907-4b89-b0da-9d68be55d3cf.png">

유저들의 일일 컨디션 리스트를 각 column별로 확인할 수 있도록 구현했습니다.
