# nest.js

- nest.js 기술 검토 진행 2023.09.19

## 검토 목적

- api 문서 자동 생성
- test 생성
- module 구성

## version

- node v18.17.1

## step

### nest.js 설치

$ npm i -g @nestjs/cli

### 새 프로젝트 생성

$ nest new project-name

- port 3000
- start 후 브라우저에서 hello world 노출 확인
- nest start --watch로 코드 변경 시 자동 적용 처리가 가능함

### 모듈 구성

- NestFactory - nestjs/core
  .create(AppModule)

- AppModule - @nestjs/common
  {
    imports: [],
    controllers: [AppController], // controller
    providers: [AppService] // service
  }
