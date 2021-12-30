# json-server
get post put delete란?(#get-post-put-delete란?)
Node.js란?(#node-js란?)
ES6이란?(#ES6이란?)
json-server의 이해 (mock server)(#json-server의-이해-(mock server))


## get post put delete란?

REST API :  웹에서 데이터를 전송 및 처리하는 방법을 정의한 인터페이스

API를 설계할때에는 URL로는 자원(resource), HTTP Method로는 행위

클라이언트가 서버에 데이터를 요청할 때 CRUD라는 4가지 타입이 있다. 
이때 CRUD는 읽기(Read), 쓰기(Create), 수정(Update), 삭제(Delete)이며 클라이언트와 서버에는 직접 명시하지 않고

Read, Create, Update, Delete > GET, POST, PUT, DELETE 라고 정의한다.

HTTP Method는 크게 GET, POST, PUT, DELETE가 대표적이다.

GET: 서버로 부터 데이터를 조회

POST: 서버에 데이터를 추가 및 작성 등

PUT: 서버의 데이터를 갱신 및 작성 등

DELETE: 서버의 데이터를 삭제

## node js란?
> **Node.js는 Chrome V8 JavaScript 엔진으로 빌드 된 JavaScript 런타임입니다.**


Node 공식 사이트에 의한 Node.js의 설명이다.

런타임은 프로그래밍 언어가 구동되는 환경인데, 전에는 브라우저(brower)에서만 작동이 되었다.

즉, Node.js는 Chrome의 V8엔진을 이용하여  javascript로 브라우저가 아니라 서버를 구축하고, 서버에서 JavaScript가 작동되도록 해주는 런타임 환경(플랫폼)이다.

Node.js의 주요 특징은

- 자바스크립트 언어 사용
- Chrome V8엔진을 이용하여 속도가 빠름
- **이벤트 기반(Event-driven)**

 이벤트가 발생할 때 미리 지정해둔 작업을 수행하는 방식

- **싱글 스레드와 뛰어난 확장성**

 ****복잡한 비동기 I/O 응용 프로그램을 싱글 스레드 JavaScript로 작성하며,

 이벤트 메커니즘은 서버가 멈추지않고 반응하도록 해주기 때문에 서버의 확장성이 뛰어나다.

- **Non blocking I/O**

Non-Blocking I/O 를 지원하면, 비동기식 프로그래밍이 가능하다.

Non-Blocking 방식은 자신이 호출되었을때 제어권을 바로 자신을 호출한 쪽으로 넘기며, 자신을 호출한 쪽에서 다른 일을 할 수 있도록 하는 것이다. 쉽게 말하면 이전 작업이 완료 될 때까지 멈추지 않고 다음 작업을 수행하는 것이다.

**Node.js의 장점과 단점**

장점

- 싱글 스레드 기반 비동기 I/O처리로 매우 빠르다.
- 브라우저 외 다른 용도의 서버로도 사용 가능하다.
- restart 시간이 1초 미안이기 때문에 프로세스가 종료되어도 빠르게 다시 시작할 수 있고, 빠른 배포나 업그레이드 작업이 가능하다.
- JS는 자바와 같은 프로그래밍 언어보다 생산성이 좋다. 같은 서버 코드를 짜는데 걸리는 시간이 적다.
- 프론트엔드와 백엔드 기술의 통합 : 프론트엔드 개발자들도 자바스크립트 기술을 가지고 서버 백엔드를 개발할 수 있게 된다.
- 싱글 스레드기 때문에 스레드간의 동기화 처리 등의 복잡한 과정을 생략할 수 있다.

단점

- 싱글 스레드 모델이기 때문에, 하나의 작업이 시간이 많이 걸리면 전체 시스템의 성능이 급격하게 떨어진다.
- 스크립트 언어의 특성 상 해당 언어가 수행되어야 에러가 나는지 확인할 수 있고, 에러가 날 경우 프로세스가 종료된다.
- 노드 전용 모듈을 사용해야 하는데, 고급 기능이 적어 세밀한 가용성 구현이 어렵다.
- 이벤트 기반 프로그래밍으로 전환하는 데에 시간이 걸린다.
- 서버 로직이 복잡할수록 비동기방식이기 때문에 CallBack Hell에 빠질 수 있다.

**Node.js 가 어울리는 웹서비스**

- 간단한 로직
- 대용량(동시에 여러 request를 처리)
- 빠른 응답시간 요구
- 빠른 개발 요구
- 비동기방식에 어울리는 서비스(네트워크 스트리밍 서비스, 채팅 서비스 등)

**Node.js를 사용하는 대표적인 회사들은 Netplix,Linkedin, Paypal, Uber, Meta(Facebook)이 있다.**

## ES6이란?


## json-server의 이해 (mock server)
