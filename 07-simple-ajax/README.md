# 07-simple-ajax

## #01. 프로젝트 생성

```shell
yarn create react-app 07-simple-sjax
```

### 1) 추가 패키지 설치

프로젝트를 VSCode로 열고, `Ctrl` + `~`를 눌러 터미널 실행

```shell
yarn add react-router-dom
yarn add qs
yarn add styled-components
yarn add axios
```

### 2) 프로젝트 생성 후 기초작업

1. **src폴더** 하위에서 App.css와 index.css, logo.svg 삭제
1. **App.js** 파일에서 App.css와 logo.svg에 대한 참조(import) 구문 제거
1. **index.js** 파일에서 index.css에 대한 참조(import) 구문 제거
1. index.js 파일에서 다음의 구문 추가
    ```js
    import { BrowserRouter } from 'react-router-dom';
    ```
1. index.js 파일에서 `<App />`을 `<BrowserRouter><App /></BrowserRouter>`로 변경
1. App.js 파일에 다음을 추가
   ```js
   import { Route, NavLink, Switch } from "react-router-dom";
   ```
   혹은
   ```js
   import { Route, Link, Switch } from "react-router-dom";
   ```

## 3) 프로젝트 실행

프로젝트를 VSCode로 열고, `Ctrl` + `~`를 눌러 터미널 실행

```shell
yarn start
```

--------------------

## #02. 예제에서 사용되는 OpenAPI

[https://newsapi.org/](https://newsapi.org/)

사이트 접속 후 메인의 **Get API Key** 버튼 클릭 후 가입양식 작성 후 APIKEY를 발급받는다.

### API 접근 방법

> https://newsapi.org/v2/top-headlines?country=kr&apiKey=발급받은KEY&catgory=???

#### category에 전달 가능한 값

| 값 | 설명 |
|----|----|
| all | 전체보기 |
| business | 비즈니스 |
| entertainment | 엔터테인먼트 |
| health | 건강 |
| science | 과학 |
| sports | 스포츠 |
| technology | 기술 |