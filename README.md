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
모임의 호스트가 모임을 생성하고 참여자들에게 링크를 공유하면, 각 참여자들이 자신의 출발 장소와 모임 가능 시간을 등록합니다. 
참여자 정보 등록을 완료하면, 취합한 참여자들의 정보를 바탕으로 중간역 및 모임 가능 시간을 추천해줍니다.

## Workflow
<img width='600px' src='https://user-images.githubusercontent.com/65700066/229273551-7638910e-2b70-428a-b4fe-6e3bc81e087d.png'>

## 기술 스택
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
├── RouteChangeTracker.ts
├── vite-env.d.ts
├── env.d.ts
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
