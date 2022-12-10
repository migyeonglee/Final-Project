<div align=center><img src=https://user-images.githubusercontent.com/97138102/206667335-4dc12a7d-59d0-437d-ae5b-2f5d30ceaefa.png ></div>

# 🥪Onetable

### 제빵 레시피 공유 사이트 제작

상세 소개: 코딩온 교육기관을 통해 진행한 세번째 프로젝트입니다. 요리 레시피 중 빵과 관련된 레시피를 공유하는 사이트를 제작하였으며, 2명씩 프론트와 백엔드로 역할을 나누어 4명이 한 조로 2주간 개발을 진행하였습니다.

## :date: 기간

2022.09.19 ~ 2022.10.04

## ERM
<img src="https://user-images.githubusercontent.com/26360179/196043616-ac2ee3b7-500b-40cf-be25-4c3dcf0ac424.png" width="600"/>
<hr />


## 💁🏻 개발담당 - FE

### 회원가입 페이지 (sweetAlert library)
![image](https://user-images.githubusercontent.com/97138102/206663573-202081da-7a02-4dc6-a575-a496f22ea4de.png)
#### Img File Upload
  -  FileReader 인스턴스 생성 : 이미지 미리보기
#### Email 
  - input type을 email로 지정
#### Password
  - input type을 password로 지정
  - 유효성 검사 
    - 8 ~ 20 자리 이내로 입력
    - 영문, 숫자, 특수문자 중 2가지 이상 혼합하여 입력
    - 동일한 문자 4번 이상 연달아 사용 불가능 
  - password 보이기 기능
    - Uicons Library 사용  -  icon
    - this를 사용하여 eye icon 클릭 시 password show/hide 가능
#### 가입하기 button 
  - focus()를 사용하여 빈칸이 있을 경우 해당 칸으로 이동
  - axios를 사용하여 formData에 담긴 정보를 back으로 넘김
  - sweetalert2를 사용하여 회원가입 실패 error 알림
---------------------------------------------------------------------------------------------------------------------    

### 로그인 페이지
![image](https://user-images.githubusercontent.com/97138102/206668883-a6bcfdab-c2fb-45b0-a613-7a2b77e15158.png)
#### Email 
  - input type을 email로 지정
#### Password
  - input type을 password로 지정
  - 유효성 검사 
    - 8 ~ 20 자리 이내로 입력
    - 영문, 숫자, 특수문자 중 2가지 이상 혼합하여 입력
    - 동일한 문자 4번 이상 연달아 사용 불가능
  - password 보이기 기능
    - Uicons Library 사용  -  icon
    - this를 사용하여 eye icon 클릭 시 password show/hide 가능
#### 로그인 Button 
   - axios를 사용하여 DB의 data와 같은 경우 성공 아닐경우 error 알림, input reset
------------------------------------------------------------------------------------------------------------------    

### 마이 페이지
![ezgif com-gif-maker (40)](https://user-images.githubusercontent.com/97138102/206687269-a15d1d90-d547-4c93-90a9-766fec89e94f.gif)

##### ejs 문법 사용
  - user 정보(프로필) 불러옴
  - 해당 user의 위시리스트 
##### 더보기 기능
  - load 시 4개씩 보이고 나머지는 숨겨짐
  - 더보기 button 클릭 시 숨겨진 리스트 4개씩 보이도록 설정
##### 수정 기능
  - axios로 수정한 formData 전송
  - sweetalert2를 사용하여 수정 성공/실패 알림

-----------------------------------------------------------------------------------------------------

### 레시피 페이지
#### Recipe Main Page
![image](https://user-images.githubusercontent.com/97138102/206679659-6b3424e8-22bc-4beb-bfc3-c312fe2b86a3.png)

##### 좋아요 순 정렬
##### 더보기 기능
  - load 시 5개씩 보이고 나머지는 숨겨짐
  - 더보기 button 클릭 시 숨겨진 리스트 5개씩 보이도록 설정
##### ejs 문법 사용
  - DB에 담긴 data의 수 만큼 recipe 추가
  
#### Recipe Item Page

<div align=center width=500px> <img src=https://user-images.githubusercontent.com/97138102/206679126-007fcdd5-54ab-4c8e-8652-4d9e22aa8b66.gif> </div>

##### recipe 좋아요 
  - Uicons Library 사용  -  icon
  - axios로 전송
##### ejs 문법 사용
  - DB와 연결되있는 recipeController에 있는 data를 불러옴
  
##### 좋아요 / 싫어요 평가, 댓글기능
  - axios로 score와 commet DB에 전송

##### 더보기 기능
  - load 시 2개씩 보이고 나머지는 숨겨짐
  - 더보기 button 클릭 시 숨겨진 리스트 2개씩 보이도록 설정

#### Recipe Register Page

![ezgif com-gif-maker (41)](https://user-images.githubusercontent.com/97138102/206835076-a837bb13-5690-49de-9ad3-293ce794e7a3.gif)

##### Img File Upload
  -  FileReader 인스턴스 생성 : 이미지 미리보기

##### 순서, 재료 추가 버튼 기능
  - click event 사용
  
##### axios 사용
  - formData에 담긴 recipe 정보 back으로 







