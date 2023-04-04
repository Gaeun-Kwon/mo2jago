# mo2jago


### 👭 이제는 진짜, 모이자고.
<img width='300px' src='https://user-images.githubusercontent.com/65700066/229273959-0eb31f19-940a-4745-9f97-4a95fe5287da.png'>

> - 프로젝트 기간: 2022.11 ~ 진행중
> - Release: 2022.12.28. (1차)
> - 팀 프로젝트
> - FE 파트 (2명)

[서비스 링크](https://mo2jago.com/)

## Service
모임의 일정과 장소를 정하는 데 편의를 제공하여 모임의 성사를 돕는 웹 서비스입니다.<br>
취합된 모임 참여자들의 정보를 바탕으로 중간역 및 모임 가능 시간을 추천해줍니다.

## FE 기술 스택
- `Typescript` 
- `React` 
- `Storybook` 

## 폴더 구조
```
src
├── main.tsx
├── index.css
├── App.tsx
├── App.css
│
├── api
│   ├── meetup.ts
│   ├── profile.ts
│   ├── edit.ts
│   ├── getGeolocation.ts
│   └── baseUrl.ts
├── components
│   ├── Alert
│   ├── Button
│   ├── SmallButton
│   ├── Icons
│   ├── Map
│   └── ScrollToTop
├── pages
│   ├── login
│   ├── create
│   ├── meetup
│   ├── profile
│   ├── edit
│   └── meetup
├── assets
│   └── ...
├── style
│   └── theme.css
├── type
│   └── index.d.ts
└── util
    ├── registDragEvent.ts
    └── envUtil.ts

```

## 서비스 모습

### 0. 서비스 온보딩
<div style='display:flex'>
  <img width='140' src='https://user-images.githubusercontent.com/65700066/229872958-b70caf49-ef72-4db5-8324-1c22aabc4920.png'>
  <img width='140' src='https://user-images.githubusercontent.com/65700066/229872964-0b054021-399b-41e2-82d6-5a7d858ed444.png'>
  <img width='140' src='https://user-images.githubusercontent.com/65700066/229872970-769fe3ab-ec6c-4e6d-9d57-1f6dc0518b76.png'>
  <img width='140' src='https://user-images.githubusercontent.com/65700066/229872973-5be35163-d127-4129-b015-67d4c3e27924.png'>
  <img width='140' src='https://user-images.githubusercontent.com/65700066/229872978-6eebb626-4553-4ad3-b0f1-400c87310341.png'>
  <img width='140' src='https://user-images.githubusercontent.com/65700066/229872982-00915767-9f23-4e43-a5a1-15db95a89649.png'>
  <img width='140' src='https://user-images.githubusercontent.com/65700066/229872986-ea3c1f7f-6b24-4180-97b5-f2c5aaf934cf.png'>
</div>

- 서비스 신규 유저에게 서비스 이해를 돕기 위한 온보딩 페이지입니다.
- `건너뛰기` 선택 시 온보딩 페이지로 가지 않고 넘어갑니다.
- `계속하기` 선택 시 온보팅 페이지로 이동합니다. 좌우 드래그를 통해 온보딩 자료를 확인할 수 있습니다.

<br>


### 1. 모임코드 입력 or 모임 생성
<div style='display:flex'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229854567-dbb78af7-1045-4f52-90df-dc8c7ba128d8.png'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229854679-b18c88fc-6eee-4f06-a2a9-57668d67bce8.png'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229854647-eb72b53c-1231-408f-a668-84d358e77847.png'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229856105-9ec5c679-be63-4dd2-9ac7-59f7a0361998.png'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229856117-eefbb493-a0f3-48a8-bb97-7a9bf9e93640.png'>
</div>

- 모임 호스트에게 전달받은 `모임코드`가 있다면, 코드를 입력해 모임 페이지에 진입합니다.
- 호스트가 되어 새로운 `모임을 생성`할 수 있습니다.

<br>

### 2. 모임 페이지


<div style='display:flex'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229858029-fac26190-21a4-48be-b21d-05c220c9beb7.png'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229858045-7f36984f-e5cd-4ad0-8a5d-d2157f862093.png'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229858051-3798e7cd-cc5d-4573-84bf-48cc32ef3db6.png'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229858039-f9059d90-bc16-4ca0-9534-58e70d52dab5.png'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229858042-41e7a70d-b552-4177-a537-e4240e4d9e4d.png'>  
</div>

- 해당 모임의 정보 - 참석자들의 정보를 취합한 `추천 시간`, `추천역`, `참석자 수` - 를 보여주는 페이지입니다.
- 장소 탭에서 지도 위에 `각 참석자들의 출발 위치`와 `추천 장소`를 시각적으로 보여줍니다.
- 우측 상단 공유 버튼을 클릭해 `초대 링크` 혹은 `초대 코드`를 복사 및 공유할 수 있습니다.

<img width='300' src='https://user-images.githubusercontent.com/65700066/229875566-1c390c77-2058-49ff-85f2-eeb09de7cf8a.png'>

- 우측 상단 설정 버튼을 클릭해 해당 `모임을 삭제`하거나, 개발자들에게 `피드백`을 보낼 수 있습니다.
- 하단 버튼을 통해 각자의 `프로필`로 진입할 수 있습니다.

<br>

### 3. 프로필 등록 및 수정

<div style='display:flex'>
  <img width='160' src='https://user-images.githubusercontent.com/65700066/229862382-aece4243-cf9a-420b-8616-1a442781d62c.png'>
  <img width='160' src='https://user-images.githubusercontent.com/65700066/229862389-105acd0e-2aeb-4951-8f09-001a0bc9feb2.png'>
  <img width='160' src='https://user-images.githubusercontent.com/65700066/229862390-3f7502df-691e-4e68-a972-5f829dcec91f.png'>
  <img width='160' src='https://user-images.githubusercontent.com/65700066/229862393-8637b143-4340-440b-9ed6-cbf34f317e8d.png'>
  <img width='160' src='https://user-images.githubusercontent.com/65700066/229862922-899681e9-b05f-4bd0-b811-012628f3bc5e.png'>  
  <img width='160' src='https://user-images.githubusercontent.com/65700066/229862397-c10f7ff2-6e50-4a17-8231-e719692bfbeb.png'>  
</div>

- 모임 참여자들이 각자의 `프로필을 등록`할 수 있습니다.
- 등록된 프로필을 선택 후, `다음 버튼`을 클릭해 본인의 정보 등록 페이지로 이동합니다.
- 각 프로필은 `수정`, `삭제`가 가능합니다.

<br>

### 4. 참여자 정보 등록 및 수정

<div style='display:flex'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229868260-e4cbcd1e-e73b-4bf1-a2b4-c5b2547b2e2b.png'>
  <img width='190' src='https://user-images.githubusercontent.com/65700066/229878031-36d53acb-349e-42e1-a5a7-bc18270eca5a.png'>
  <img width='195' src='https://user-images.githubusercontent.com/65700066/229868271-0ea52b59-131d-4b94-a876-870a477bcd9e.png'>
</div>

- 자신의 `출발 장소`를 등록 및 수정할 수 있습니다.
- `장소 검색` 시 하단에서 장소 검색 시트가 올라와, 장소명으로 검색할 수 있습니다. 장소까지의 거리와 상세 주소가 표시되며 최대 45개까지 무한 스크롤하며 장소 정보를 받아볼 수 있습니다.
- 만남 장소를 등록하지 않는 경우, `어디든 상관없어요` 버튼을 클릭합니다.
- 하단 지도에서 현재 모임 참석자들의 출발지 현황과, 추천 장소를 보여줍니다.
- 장소 정보를 입력한 후, `완료` 버튼을 눌러 장소 등록을 완료합니다. 
등록 완료 시 모임 페이지로 이동합니다.



