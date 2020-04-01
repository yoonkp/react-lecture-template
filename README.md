# react-lecture-template

이젠아카데미 수업용 리액트 예제 프로젝트 템플릿 입니다.

[copyright&copy;itpaper.co.kr](https://blog.itpaper.co.kr)

## #01. 설치할 프로그램
1. Node.js
   - npm 명령
   - react가 내부적으로 테스트 환경 구동을 위해 사용
   - [https://nodejs.org/en/](https://nodejs.org/en/)
1. Yarn
   - npm이 개선된 형태.
   - [https://yarnpkg.com/](https://yarnpkg.com/)
1. 에디터
   - Visual Studio Code
   - [https://code.visualstudio.com/](https://code.visualstudio.com/)


## #02. 프로젝트 생성

### 1) 작업폴더에서 명령창 열기

폴더 빈 곳에서 Shift + 마우스 우클릭 후 **여기에 Powershell 열기** 선택

### 2) 패키지 관리자 (npm, yarn)

개발과정에서 필요한 패키지(혹은 플러그인)의 다운로드, 업데이트, 제거 등을 담당하는 명령어.

npm과 yarn중 하나만 수행하면 된다. (yarn 추천)

#### 패키지 설치하기
```shell
yarn add 패키지이름
```

혹은

```shell
npm install 패키지이름 --save
```

#### 패키지 삭제하기

```shell
yarn remove 패키지이름
```

혹은

```shell
npm uninstall 패키지이름 --save
```

### 3) 리액트 프로젝트 생성하기

```shell
yarn create react-app 프로젝트이름
```

혹은

```shell
npm create react-app 프로젝트이름
```

> 프로젝트 이름에 대문자 사용X


### 4) 생성된 프로젝트 실행하기

#### 명령창 상에서 프로젝트 폴더 안으로 진입

```shell
cd 프로젝트이름
```

#### 실행하기

```shell
yarn start
```
혹은
```shell
npm start
```

-----------------

## #03. VSCode 확장기능 설치

### 1) 기본설치
- Korean Language Pack for Visual Studio Code
- Markdown All in One
- Markdown Preview Github Styling

### 2) Javascript 및 React 도구
- ESLint : 자바 스크립트 문법 및 코드 스타일 검사 도구
- Reactjs Code Snippets : 리액트 컴포넌트 및 라이프사이클 함수를 작성할 때 단축 단어를 사용하여 간편하게 코드를 자동으로 생성해 낼 수 있는 코드 조각 모음. 제작자가 charalampos karypidis인 것 추천
- Prettier-Code formatter: 코드 스타일을 자동으로 정리해 주는 도구


### 3) ESLint 설정

명령프롬프트에서 다음의 명령들을 수행한다.

`WinKey+R` > `cmd` 입력 후 `Shift`+`Enter`

```shell
npm install -g eslint
npm install --save-dev babel-eslint
npm install --save-dev eslint-plugin-react
```

### 4) VScode 설정 추가

```json
"javascript.validate.enable": false,
"eslint.enable": true,
"jshint.options": {
    "esversion": 6
}
```
