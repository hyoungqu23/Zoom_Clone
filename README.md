# Zoom Clone Coding using Node.js, WebRTC and Websockets
## 개발 환경 설정
### npm 프로젝트 시작하기
npm 프로젝트를 다음 명령어로 시작하면, package.json 파일이 루트 디렉토리에 생성된다.
```
npm init -y
```
이후 package.json 파일을 열어 다음 코드를 제거한다.
```json
"main": "index.js",
"scripts": {
  "test": "echo \"Error: no test specified\" && exit 1"
},
```
### nodemon 설치
터미널에 다음 명령어를 통해 nodemon을 설치할 수 있다. 이후, 루트 디렉토리에 nodemon.json 파일을 생성한다.
```
npm i nodemon -D
```
```json
{
  "exec": "babel-node src/server.js"
}
```
### babel 설치
루트 디렉토리에 babel.config.json 파일을 생성하고 다음 명령어를 통해 설치한다.
```
npm i @babel/core @babel/cli @babel/node @babel/preset-env -D
```
```json
{
  "presets": ["@babel/preset-env"]
}
```
### package.json 수정
다음 코드를 추가해 `dev` 명령어로 `nodemon`을 호출하게 한다.
```json
"scripts": {
  "dev": "nodemon"
},
```
### express.js 설치
```
npm i express
```
### pug 설치
```
npm i pug
```
