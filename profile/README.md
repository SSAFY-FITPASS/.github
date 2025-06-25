# VUE 관통 PJT
> **기간:** 2024-11-04 ~ 2024-11-17
> 
> **팀 구성:** 김지윤, 나혜원  
> 
> **소속:** 서울 9반
<br/>

## I. Introduction
### 프로젝트 소개
- 프로젝트 이름: FITPASS
- 목적: FITPASS는 FITNESS와 PASSPORT의 결합어로, 사용자가 운동과 여행의 경험을 디지털 여권 형태로 기록하고 공유할 수 있는 서비스를 제공합니다.
- 주요 기능:
    - 운동 기록: 여행 중 방문한 피트니스 센터, 운동 장소, 또는 액티비티를 기록할 수 있습니다.
    - 여행 기록: 여행지에서의 활동과 경험을 상세히 기록 및 저장할 수 있습니다.
    - 커뮤니티: 사용자가 서로의 여정을 공유하고, 영감을 받을 수 있는 커뮤니티 공간을 제공합니다.
    - 개인 대시보드 관리: 자신의 운동 목표와 여정을 시각적으로 관리할 수 있는 사용자 대시보드를 제공합니다.
- 예상 사용자:
    - 새로운 액티비티(운동)을 경험하기 위해 여행을 떠나는 사람들.
    - 여행지에서의 독특한 경험을 기록하고자 하는 사람들.
    - 운동과 여행을 결합한 라이프스타일을 지향하는 사람들.
    - 여행 및 운동 경험을 커뮤니티와 공유하고, 다른 사람의 여정을 통해 영감을 얻고자 하는 사람들. 

### 주요 기술 스택:
- Frontend: Vue 3, Vuetify
- 상태 관리: Pinia
- 스타일링: Vuetify, CSS
- 지도 API: Kakao Maps

<br/>

## II. Features
### 프로젝트 디렉토리 구조
```
📦src
 ┣ 📂assets
 ┃ ┣ 📜base.css
 ┃ ┣ 📜login.png
 ┃ ┣ 📜logo.png
 ┃ ┣ 📜logo.svg
 ┃ ┣ 📜main.css
 ┃ ┣ 📜map.jpg
 ┃ ┗ 📜profile.png
 ┣ 📂components
 ┃ ┣ 📂adminpage
 ┃ ┃ ┣ 📜AdminListView.vue
 ┃ ┃ ┣ 📜AdminPageView.vue
 ┃ ┃ ┣ 📜AdminRequestView.vue
 ┃ ┃ ┗ 📜AdminSportView.vue
 ┃ ┣ 📂community
 ┃ ┃ ┣ 📜CommunityPageView.vue
 ┃ ┃ ┣ 📜CommunityPostsView.vue
 ┃ ┃ ┗ 📜FriendListView.vue
 ┃ ┣ 📂main
 ┃ ┃ ┣ 📜AdminDialogCard.vue
 ┃ ┃ ┣ 📜FeaturesSection.vue
 ┃ ┃ ┣ 📜HeaderSection.vue
 ┃ ┃ ┣ 📜MainPageView.vue
 ┃ ┃ ┗ 📜Navbar.vue
 ┃ ┣ 📂myHome
 ┃ ┃ ┣ 📜KaKaoMapView.vue
 ┃ ┃ ┣ 📜MyPageView.vue
 ┃ ┃ ┣ 📜MyPostsView.vue
 ┃ ┃ ┗ 📜MyRecordsView.vue
 ┃ ┣ 📂profile
 ┃ ┃ ┣ 📜ProfileEditView.vue
 ┃ ┃ ┗ 📜ProfileView.vue
 ┃ ┣ 📂write
 ┃ ┃ ┣ 📜KakaoPlaceRegistView.vue
 ┃ ┃ ┗ 📜WritePageView.vue
 ┃ ┣ 📜Login.vue
 ┃ ┣ 📜Logo.vue
 ┃ ┣ 📜MainPage.vue
 ┃ ┗ 📜Singup.vue
 ┣ 📂plugins
 ┃ ┗ 📜vuetify.js
 ┣ 📂router
 ┃ ┗ 📜index.js
 ┣ 📂stores
 ┃ ┣ 📜counter.js
 ┃ ┗ 📜user.js
 ┣ 📂views
 ┃ ┣ 📜AboutView.vue
 ┃ ┗ 📜HomeView.vue
 ┣ 📜.env.local
 ┣ 📜App.vue
 ┗ 📜main.js

```
### 프로젝트 화면
#### 첫 화면
![firstPage](images/firstPage.png)
#### 회원가입 페이지
#### 로그인 페이지
![logIn](images/logIn.png)
#### 대시보드 페이지
![main-1](/uploads/16a06cd63af8e965d7f29d8c67995f36/main-1.png)<br>
![main-2](/uploads/d7647ba69df1c22ddd8e0311f41309b9/main-2.png)<br>
관리자 요청 클릭 시 화면 <br>
![admin-req](/uploads/3779e55376b73bcf37a8586cc4800f9b/admin-req.png)
#### 커뮤니티 페이지
![commu](/uploads/0863c6369f1a95a355529d06faaaa571/commu.png)
#### 게시글 작성 페이지
![write](/uploads/ecb1eea4f74688c8e421fb0f1e3d6ee0/write.png) <br>
주소를 입력하고 검색하면 관련 주소가 표시된 지도 이미지가 보입니다.<br>
![write-2](/uploads/e07fba075176c22db415b4a141a7ea79/write-2.png)
#### 내 정보 페이지
![myProfile](images/myProfile.png)
#### 관리자 페이지 - 1
![adminPage1](images/adminPage1.png)
#### 관리자 페이지 - 2
![adminPage2](images/adminPage2.png)
#### 관리자 페이지 - 3
![adminPage3](images/adminPage3.png)

<br/>

## III. 기능 구현

1. 사용자 대시보드 관리

    사용자는 개인 대시보드에서 이전에 방문한 여행지, 운동 장소, 운동한 총 시간 둥울 시각적으로 한 눈에 볼 수 있습니다.
    또한, 지도를 이용해 여행지와 운동 장소를 직관적으로 탐색할 수 있습니다.

2. 게시물 작성 및 커뮤니티 기능

    게시물 작성: 사용자가 글을 작성하여 저장할 수 있습니다. <br/>
    커뮤니티: 작성된 게시물을 다른 사용자와 공유 및 조회할 수 있습니다.
3. 관리자 요청 기능

    사용자는 관리자에게 특정 요청을 보낼 수 있습니다.
4. 친구 기능 

    사용자 검색을 통해 친구 요청을 보낼 수 있으며 친구 목록을 관리할 수 있습니다.


## IV. 프로젝트 회고

### 김지윤
> 맨땅에서 처음부터 해보는 프로젝트는 처음이라 긴장 반 기대 반으로 시작한 프로젝트였습니다.
> 초기에는 아이디어를 구체화하고 구상하는 데 고민이 많았지만, 페어의의 협업과 문제 해결 과정을 통해 프로젝트의 방향성을 확립할 수 있었습니다.
> 특히, 화면 설계 단계에서 각 컴포넌트들을 어떻게 분리할 것인지 고민하며 더 나은 서비스를 제공하기 위해 많은 노력을 기울였습니다. <br/>
> 화면 구현 과정에서 예상치 못한 어려움을 겪기도 했지만, 페어와 함께 이를 해결해 나가며 프론트엔드에 대한 이해가 한층 깊어졌습니다. <br/>
> 프로젝트 기획부터 설계, 구현까지 처음부터 해볼 수 있었던 뜻 깊은 경험이었습니다. 최종 프로젝트까지 남은 부분을 완성하고, 부족한 점들을 채워나가 유종의 미를 거두고 싶습니다.

### 나혜원 



## 추천 IDE 설정  

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

## 프로젝트 설정 

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```
