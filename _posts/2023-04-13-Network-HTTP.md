---
title: HTTP _1(HTTP란)
author: 
date: 2023-04-13 00:10:00 +0800
categories: [Network, HTTP]
tags: [Network]
render_with_liquid: false
---



## HTTP

 HTTP란 : 
 일명 `하이퍼텍스트 전송 프로토콜`은 하이퍼미디어 문서를 전송하기 위한 애플리케이션 레이어(OSI 7단계: 호스트가 사용하는 공유통신 프로토콜 및 인터페이스 방법을 지정하는 추상화 계층) 프로토콜이며 웹브라우저와 웹서버 간의 통신을 목적으로 설계됨.
 (여기서 하이퍼미디어 문서는 예를 들면 텍스트 비디오,스크립트 등 )
 
HTTP는 클라이언트가 요청하기 위해 연결을 연 다음에 응답을 받을때까지 대기하는 `클라이언트-서버` 모델을 따름
또한 HTTP는 무상태 프로토콜이며 서버가 두요청간에 어떠한 상태로 유지하지 않음 

- HTTP 특징 :
1. 사람들이 읽기 간단하게 고안됨
2. 확장성 (HTTP 헤더는 확장하기 쉽움)
3. 상태는 없지만 세션은 있음 (HTTP 핵심은 상태가 없는것이지만 HTTP쿠키는 상태가 있는 세션을 만들수 있도록함 )


## HTTP 기반 API
user agent(예: 브라우저)와 서버 간의 통신을 교환하는데 사용하는 XMLHttpRequest API 및 FETCH API 가 있다. (fetCH기능이 더 강력하고 유연하다고 함 )

## HTTP 로 제어가능한것
1. 캐시
2. ORIGIN 제약사항 강화
3. 인증
4. 세션

## HTTP 흐름


## 참조
- HTTP 기반 시스템 구성요소 
1. USER-AGENT
2. WEB SERVER
3. PROXY

