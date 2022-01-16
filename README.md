<div align ="center">
  항해99 5기 5조 1주차 미니프로젝트, Show Your Bucekt
</div>

* * *

#### 프로젝트 소개
> 새로운 한 해 동안 자신이 하고 싶은 Bucket List를 기록하고 공유하는 플랫폼 입니다.

#### 🎥프로젝트 시연 영상
> https://youtu.be/KtNottkJ_dk

#### 🔗프로젝트 URL
> http://showyourbucket.shop

#### 제작 기간 & 팀원 소개
>제작 기간: 2022.01.10 ~ 2022.01.13  
>팀원🧑‍💻👩‍💻: 오성택, 김기덕, 정재연, 김현지
* * *
<div align ="center">
  <b>
 Tech Stack
  </b>
</div>

<div align ="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=white"> <img src="https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=CSS3&logoColor=white"> <img src="https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jQuery&logoColor=white"></br> <img src="https://img.shields.io/badge/Jinja2-B41717D?style=for-the-badge&logo=Jinja&logoColor=white"> <img src="https://img.shields.io/badge/mongodb-47A248?style=for-the-badge&logo=MongoDB&logoColor=white"> <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=Flask&logoColor=white"> <img src="https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=AWS&logoColor=white"> <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=white"> <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=BootStrap&logoColor=white">
</div>
<br></br>
<div align ="center">
  <b>
  Cowork Tools
  </b>
</div>  
<div align ="center">
  <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white"> <img src="https://img.shields.io/badge/slack-4A154B?style=for-the-badge&logo=slack&logoColor=white"> <img src="https://img.shields.io/badge/kakaotalk-FFCD00?style=for-the-badge&logo=kakaotalk&logoColor=white">
</div>

* * *
## 🖥 API 설계
<img width="475" alt="api" src="https://user-images.githubusercontent.com/91252981/149308577-bb5924d3-8ab8-4e3f-9ea7-9ddb0986c265.png">

* * *
## 📷Screenshot

### Main Page
<img src="https://user-images.githubusercontent.com/91252981/149301569-a0fc96e7-7f5c-4fd8-8abc-d12e5a14ddde.png">

### Login Page
<img src="https://user-images.githubusercontent.com/91252981/149301879-420e17b5-9f0d-4067-addc-6c36487357e1.png">

### Register Page
<img src="https://user-images.githubusercontent.com/91252981/149301877-1df95947-c935-4a59-853d-b20a9e723197.png">

### Posting Page
<img src="https://user-images.githubusercontent.com/91252981/149302790-d9cf2664-e05d-49e0-b1cc-8067d832c26f.png">

### Modal
<img src="https://user-images.githubusercontent.com/91252981/149306564-15a6d2cc-aa8e-4fa7-86b5-b3ed0ee30bbc.png">

* * *
## 📌 Trouble Shooting

<details>
    <summary>1. preview를 띄어주는 이미지 업로드 기능 구현 시, 이미지가 변경이 되지 않고 preview 하단에 이미지가 쌓이는 문제</summary></br>
     
     개발자 도구에서 확인 해보니 container.appendChile(newImage)로 인해 image-show div 에 추가로 이미지가 계속 쌓이고 있는 점을 발견했다
     container.removeChild(container.children[0]) 조건으로 첨부 파일이 있을 때는 기존 이미지를 삭제 해준 후 
     새로운 이미지를 추가 하는 것으로 해결 
<!-- summary 아래 한칸 공백 두고 내용 삽입 -->

</details>
</br>
<details>
  <summary>2.ajax GET 요청으로 받은 data를 modal popup으로 다시 띄어줄 때 고유 id값을 불러오지 못하는 문제</summary></br>
  
    api 쪽에서 _id 값을 string 형태로 받아온 후, 다시 client 쪽에서 modal popup function으로 넘겨 준 뒤
    modal popup function 에서 _id 값을 api 쪽에 넘겨서 해당 데이터 불러오는 것으로 해결
    
</details>
</br>
<details>
  <summary>3.토큰이 만료되면 자동 로그아웃 되는 기능 구현 시, 토큰값이 만료는 되지만 계속 남아있어서 자동 로그아웃 기능 구현 실패</summary></br>
  
    토큰이 만료되는 시간에 맞추어 토큰값을 삭제하는 방법으로 토큰값이 없을 경우 자동 로그아웃 시키고 메인페이지로 이동하게끔 해결
    
</details>

