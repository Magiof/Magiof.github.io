---
title: Why Node.js?
tags: [Node.js, Nest.js]
style: fill
color: secondary
description: Benefits of using Node.js as a backend server.
---

Source: [네이버포스트](https://post.naver.com/viewer/postView.nhn?volumeNo=26678816&memberNo=2521903), [youtube](https://youtu.be/QcNqfvMeWow)

## What is Node.js
![Node.js](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Node.js_logo.svg/2560px-Node.js_logo.svg.png)

위키백과에서 Node.js는 다음과 같이 정의되고 있습니다.
``` text
Node.js는 확장성 있는 네트워크 애플리케이션(특히 서버 사이드) 개발에 사용되는 소프트웨어 플랫폼이다.
작성 언어로 자바스크립트를 활용하며 Non-blocking I/O와 단일 스레드 이벤트 루프를 통한 높은 처리 성능을 가지고 있다.
내장 HTTP 서버 라이브러리를 포함하고 있어 웹 서버에서 아파치 등의 별도의 소프트웨어 없이 동작하는 것이 가능하며,
이를 통해 웹 서버의 동작에 있어 더 많은 통제를 가능케 한다.
```
Node.js는 2009년 처음 등장한 자바스크립트 런타임입니다.<br>
Node.js가 등장하기 전까지 자바스크립트는 대표적인 클라이언트 개발 언어로만 여겨졌는데요.<br>
JavaScript Everywhere라는 기조에 따라 만들어진 Node.js는 자바스크립트로 클라이언트와 서버를 모두 개발할 수 있어 개발자들에게 많은 관심을 받고 있습니다.<br>
실제로 넷플릭스, 페이스북, 링크드인 등 거대 글로벌 기업에서도 웹 서비스 개발에 Node.js를 사용하고 미국 항공 우주국 NASA에서도 Node.js를 활용하고 있습니다.
<br>
<br>
<br>
<br>

## 1. NASA manages the lifecycle data of space suits using Node.js.

![NASA x Node](https://post-phinf.pstatic.net/MjAxOTEwMjhfMTUg/MDAxNTcyMjQ3NjY2MTI5.5L9RHYcTvjbxMm9MNb2JTD3d3VYzBld_KZzQsJLCFI0g.Y6Y3Ay9Cn_Zylg64Pa_UiEng-1oUJGtRyIrL86WgNcUg.PNG/image.png?type=w1200)

NASA는 2013년 우주 비행사의 헬멧에 있던 물이 누수 되어 큰 사고로 이어질뻔한 사건을 경험한 이후, 우주복의 전체 라이프사이클 데이터를 하나의 클라우드에서 통합 관리할 수 있도록 변경하고, 클라우드에 데이터를 전송하는 과정에 Node.js를 활용하고 있습니다.
​
이전에는 하드웨어 기반 데이터 처리로 인해 여러 곳에 분산된 데이터베이스를 수집하는 작업이 천문학적인 규모의 작업으로 수행되었지만, 클라우드 기반의 컨테이너에서 동작하는 **마이크로서비스 아키텍처** 구조를 이용하고, **각각의 애플리케이션을 API로 연결하여 모든 정보를 하나의 데이터베이스에 접근**하여 확인할 수 있어 <span style="background-color:#fff5b1"> <span style="color:black"> **접근 시간이 300% 단축**</span></span> 되었다고 합니다.
<br>
<br>
<br>
<br>

## 2. Netflix migrating 1/2 of their api to Node.js.

![Netflix x Node](https://miro.medium.com/max/1400/1*bp-HD0SALx8ud88kJcesQw.jpeg)

Netflix는 Node.js의 이점을 활용하여 프로덕션 환경을 구현한 최고의 사례이며 경제적으로나 성과면에서 엄청난 성과를 거두었습니다.
 이전 Netflix는 서버 측에서 Java를 사용하고 프론트엔드 측에서는 JavaScript를 사용했기 때문에 개발자는 두 언어를 모두 이해하고 프로그래밍, 에러 핸들링, 디버깅 등을 두 번씩 해야했습니다.

Netflix가 spring에서 Node.js로 migration한 주된 이유는 **프론트엔드 측과 서버 측 모두에서 같은 언어를 사용하기 위함**입니다. 또한 Node.js에는 **npm**이라는 방대한 오픈 소스에 커뮤니티에 대부분이 무료 소스인 많은 모듈이 있으며, 결과적으로 Netflix는 Node.js 도입 후 단일 페이지 어플리케이션을 생성하기 위해 <span style="background-color:#fff5b1"> <span style="color:black"> **40분 이상 걸리던 시작 시간을 1분 미만으로 줄였습니다.**</span></span> 
<br>
<br>
<br>
<br>

## 3. LinkedIn migrate to NodeJS from Ruby.

![LinkedIn](https://www.pixelstech.net/article/images/LINKEDIN.png)

2011년, LinkedIn은 Ruby로 작성된 60,000줄의 코드를 성능 향상을 목표로 Node.js와 함께 핵심 모바일 서비스를 재구축하기 시작했습니다.
그 결과로 LinkedIn은 **2000줄의 JavaScript**코드만을 갖게 되었습니다.
이러한 감소의 가장 큰 이유는 기본적으로 프레임워크가 없기 때문입니다. 즉, 그 안에 조작된 부분(추상화, 객체화)이 많지 않다는 것을 의미합니다.

두 번째 큰 이유는 우리에게 중요한 변화로 판명된 객체 지향 접근 방식과 달리, 더 기능적인 접근 방식과 관련이 있습니다. Ruby에서 자연스러운 경향은 본질적으로 모든 의사소통과 유형을 포장하는 객체를 만드는 것입니다. Ruby는 실제로 기능적인 언어이지만 자바스크립트보다 클래스와 객체에 대한 개념이 훨씬 강합니다. 
그래서 LinkedIn의 초기 코드 베이스에는 심한 구성요소화와 더불어 리팩터링 할 수 있으며 재사용성을 강조하여 만들어진 클래스와 객체의 많은 레이어가 있었습니다.
LinkedIn 팀은 `하지만 돌이켜보면, 우리는 정말로 그것의 대부분이 필요하지 않았다.` 라고 말합니다.

결과적으로 LinkedIn의 Node.js로의 migration을 이끈 Kiran Prasad는 일련의 작업들이 LinkedIn의
<span style="background-color:#fff5b1"> <span style="color:black"> **성능을 유지하고 확장의 용이성을 유지**</span></span> 할 수 있게 됐다고 말했습니다.
<br>
<br>
<br>
<br>

## Benefits using Node.js as a backend server.

Node.js를 백엔드 서버로 사용하는 것에는 여러 가지 이점이 있습니다.

1. 빠르고 확장성이 좋음: Node.js는 V8 JavaScript 엔진 위에 구축되어 있어 처리 속도가 빠르다는 특징이 있습니다. 이로 인해 Node.js는 확장성이 뛰어나고 고성능 애플리케이션을 구축하기에 좋은 선택입니다.

1. 단일 언어: Node.js는 프론트엔드 개발에서도 사용되는 JavaScript를 사용합니다. 이는 개발자들이 프론트엔드와 백엔드 모두에 같은 언어를 사용할 수 있으므로 개발 프로세스가 더욱 효율적이고 컨텍스트 전환의 필요성이 줄어듭니다.

1. Non-blocking I/O: Node.js는 Non-blocking I/O를 사용하여 프로그램 실행을 차단하지 않고 동시에 여러 요청을 처리할 수 있습니다. 이로 인해 Node.js는 실시간 애플리케이션을 구축하거나 고트래픽 웹사이트를 처리하는 데 좋은 선택입니다.

1. 방대한 커뮤니티: Node.js는 크고 활발한 개발자 커뮤니티를 가지고 있으며, 개발자들이 사용할 수 있는 많은 리소스와 도구가 있습니다. 이는 빠르게 버그와 이슈를 식별하고 해결할 수 있다는 것을 의미합니다.

1. 마이크로서비스 아키텍처(MSA): Node.js는 마이크로서비스 아키텍처를 구축하기에 적합하며, 단일 모놀리식 애플리케이션보다 더 쉽게 확장 및 유지보수할 수 있습니다.
