# json-server
* [get post put delete란?](#get-post-put-delete%EB%9E%80)
* [Node.js란?](#node-js%EB%9E%80)
* [ES6이란?](#es6%EC%9D%B4%EB%9E%80)
* [json-server의 이해](#json-server%EC%9D%98-%EC%9D%B4%ED%95%B4)


## get post put delete란?

REST API :  웹에서 데이터를 전송 및 처리하는 방법을 정의한 인터페이스

API를 설계할때에는 URL로는 자원(resource), HTTP Method로는 행위

클라이언트가 서버에 데이터를 요청할 때 CRUD라는 4가지 타입이 있다. 
이때 CRUD는 읽기(Read), 쓰기(Create), 수정(Update), 삭제(Delete)이며 클라이언트와 서버에는 직접 명시하지 않고

Read, Create, Update, Delete > GET, POST, PUT, DELETE 라고 정의한다.

HTTP Method는 크게 GET, POST, PUT, DELETE가 대표적이다.

GET: 서버로부터 데이터를 조회

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

 복잡한 비동기 I/O 응용 프로그램을 싱글 스레드 JavaScript로 작성하며,

 이벤트 메커니즘은 서버가 멈추지않고 반응하도록 해주기 때문에 서버의 확장성이 뛰어나다.

- **Non blocking I/O**

Non-Blocking I/O 를 지원하면, 비동기식 프로그래밍이 가능하다.

Non-Blocking 방식은 자신이 호출되었을때 제어권을 바로 자신을 호출한 쪽으로 넘기며, 자신을 호출한 쪽에서 다른 일을 할 수 있도록 하는 것이다. 쉽게 말하면 이전 작업이 완료 될 때까지 멈추지 않고 다음 작업을 수행하는 것이다.

**Node.js의 장점과 단점**

장점

- 싱글 스레드 기반 비동기 I/O처리로 매우 빠르다.
- 브라우저 외 다른 용도의 서버로도 사용 가능하다.
- restart 시간이 1초 미만이기 때문에 프로세스가 종료되어도 빠르게 다시 시작할 수 있고, 빠른 배포나 업그레이드 작업이 가능하다.
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
ECMAScript 6는 ECMAScript의 최신 버전이며, ECMA-262 규격을 따른다.

ES6은 ECMA-262의 6판이라고 보면 된다.

ECMAScript은 *자바스크립트 언어의 표준 언어*이다.

**JavaScript와 ECMAScriptd의 차이**

**JavaScript**

ECMAScript 사양을 준수하는 범용 스크립팅 언어

**ECMAScrip**

Ecma 인터내셔널에 의해 제정된 ECMA-262 기술 규격에 의해 정의된 범용 스크립트 언어

**ES6 문법**

* const and let
- Arrow functions(화살표 함수)
- Template Literals(템플릿 리터럴)
- Default parameters(기본 매개 변수)
- Array and object destructing(배열 및 객체 비구조화)
- Import and export(가져오기 및 내보내기)
- Promises(프로미스)
- Classes(클래스)

- ### const and let

`const`는 변수 선언을 위한 ES6의 새로운 키워드이다.

 `const`는 `var`보다 강력하고 일단 사용되면 변수를 다시 할당할 수 없다. 

즉, 객체와 함께 사용할 때를 제외하고는 **변경 불가능한 변수**

```jsx
// ES5
    var name = 'lemming'
    console.log(name) // lemming

    var name = 'javascript'
    console.log(name) // javascript
```

변수를 한 번 더 선언했음에도 불구하고, 에러가 나오지 않고 다른 값이 출력된다.

코드가 많아진다고 치면 어디에서 어떻게 사용 될지도 파악하기 힘들뿐더러 값이 바뀔 우려가 있다.

그래서 ES6 이후, 이를 보완하기 위해 추가 된 변수 선언 방식이 `let` 과 `const` 이다.

위 코드에서 변수 선언 방식만 다르게 하면

```jsx
// ES6
    let name = 'lemming'
    console.log(name) // lemming

    let name = 'javascript'
    console.log(name)
    // Uncaught SyntaxError: Identifier 'name' has already been declared
```

변수 재선언이 되지 않는다.
추가로 `let`과 `const`의 차이는 
`let` 은 변수에 재할당이 가능

```jsx
    let name = 'lemming'
    console.log(name) // lemming

    let name = 'javascript'
    console.log(name)
    // Uncaught SyntaxError: Identifier 'name' has already been declared

    name = 'nodejs'
    console.log(name) //nodejs
```

`const`는 변수 재선언과 변수 재할당 모두 불가능하다

```jsx
    const name = 'lemming'
    console.log(name) // lemming

    const name = 'javascript'
    console.log(name)
    // Uncaught SyntaxError: Identifier 'name' has already been declared

    name = 'nodejs'
    console.log(name)
    //Uncaught TypeError: Assignment to constant variable.
```

하지만 인터넷 익스플로러에서는 `let` 과 `const`는 지원하지 않으므로  `var`을 사용해야 한다.

- ### Arrow functions(화살표 함수)

ES6에서는 익명 함수를 더 간단하게 생성할 수 있는 방법으로 화살표 함수를 제공한다.

```jsx
let name = () => {
    console.log("lemming");
};

name();
console.log(name);
//출력 = > lemming
```

대부분의 익명 함수 코드는 화살표 함수로 대체할 수 있고,

function 키워드 대신 화살표(=>)를 사용하여 보다 간략한 방법으로 함수를 선언할 수 있다.

- ### Template Literals(템플릿 리터럴)

문자열을 연결하기 위해 더하기(+) 연산자를 사용할 필요가 없고, 백틱(`)을 사용하여 문자열 내에서 변수를 사용할 수도 있다.

```jsx
// ES5
function lemming() {
	return '안녕하세요' + name + '이번년도의 너의 나이는' + age + '살 이다!';
}

console.log(myFunc1('레밍', 20));
// 출력 => 안녕하세요 레밍 이번년도의 너의 나이는 20살 이다!
```

변수나 코드를 표현할 때는 ${}의 중괄호로 감싸준다.

```jsx
// ES6
const lemming= (name, age) => {
	return `안녕하세요 ${name}, 내년의 너의 나이는 ${age}살 이다!`;
};

console.log(lemming('레밍', 21));
// 출력 => 안녕하세요 레밍, 내년의 너의 나이는 21살 이다!
```

번거로움도 줄어들고 읽기도 편해졌다.

- ### Default parameters(기본 매개 변수)

매개 변수를 쓰지 않은 경우 매개 변수가 이미 기본값에 정의되어 있어 정의되지 않은 오류가 반환되지 않는다.

```jsx
function me(a){ 
return a;
}
console.log(js()); // undefined
```

매개변수를 넣지 않고 함수를 그냥 실행해 버리면 undefined를 그대로 반환하는것이다.

그래서 이를 방지하기 위해 매개변수에 기본값을 사용하면 된다.

```jsx
function me(a = 'lemming'){
return a; 
} console.log(me()); // lemming
```

동일하게 호출을 하였지만 기본 매개변수의 기본값을 넣었기 때문에 기본값이 출력되는 것을 볼 수 있다.

함수 매개변수 기본값을 사용할 때에 **하나 주의할 점은 매개변수가 undefined 일 때만 작동**한다.

- **Array and object destructing(배열 및 객체 비구조화)**

**배열**

```jsx
const subjectList = ["Javascirpt", "Java", "Python"];
const Javascirpt = subjectList[0];
const Java = subjectList[1];
const Python = subjectList[2];
console.log(Javascirpt); // Javascirpt
console.log(Java); // Java
console.log(Python); // Python
```

배열의 값을 각각 변수에 할당 하려면 위처럼 각각 하나씩 지정해 줘야 하는데 이 과정은 번거롭기도 하고 코드가 복잡해 보인다.

```jsx
const [Javascirpt, Java, Python] = ["Javascirpt", "Java", "Python"];
console.log(Javascirpt); // Javascirpt
console.log(Java); // Java
console.log(Python); // Python
```

비구조화 할당을 이용하면 간단하게 작성할 수 있다.

**객체**

```jsx
const subject = {
  Javascirpt: "Javascirpt",
  Java: "Java",
  Python: "Python"
};
const Javascirpt = animals.Javascript;
const Java = subject.Java;
const Python = subject.Python;
console.log(Javascirpt); // Javascirpt
console.log(Java); // Java
console.log(Python); // Python
```

객체도 배열과 마찬가지로 일일히 값을 따로 넣어주려면 번거롭다.

```jsx
const {Javascirpt, Java, Python} = {
  Javascirpt: "Javascirpt",
  Java: "Java",
  Python: "Python"
};
console.log(Javascirpt); // Javascirpt
console.log(Java); // Java
console.log(Python); // Python
```

문장이 조금 더 간결해졌다!

- ### Import and export(가져오기 및 내보내기)

`export`를 사용하면 다른 JavaScript 구성 요소에 사용할 모듈을 내보낼 수 있습니다. 우리는 그 모듈을 우리의 컴포넌트에 사용하기 위해 가져오기 `import`를 사용합니다.

```jsx
//data.js
export default function data(name, age) {
	return `안녕하세요 ${name}, 나이는 ${age}살!`;
}
```

그리고 `profile.js`에서 이 기능을 사용하려면 `import`만 사용합니다.

```jsx
//profile.js
import data from './data';

console.log(data('lemming', 20));
// 출력 => 안녕하세요 lemming, 나이는 20살!
```

두 개 이상의 모듈을 가져오려면, 중괄호에 넣으면 된다.

```jsx
import { data, userProfile, getPosts } from './data';

console.log(data('lemmig', 20));
console.log(userProfile);
console.log(getPosts);
```

- ### Promises(프로미스)

싱글 스레드인 자바스크립트에서 비동기 처리를 위해서 콜백(callback)을 사용해왔는데,

콜백이 사용되는 경우가 많아지면서 단점이 생겼다.

단점은 비동기 처리를 순차적으로 실행할 필요가 있는 경우에 비동기 처리를 중첩시켜서 표현하므로 **에러, 예외처리가 어렵다**는 것과 **중첩으로 인한 복잡도가 증가**하는 것이다.

이 두 가지의 단점을 고친 것이 프로미스이다.

```jsx
const promise1 = function(param){
return new Promise(function(resolve,reject){
if(param){
resolve("rem");
}
else{
reject("lemming");
}
});
}
//프로미스 실행
promise1(true).then(function(result){
console.log(result);//rem
},function(err){
console.log(err);//lemming
});

```

비동기함수를 만들어서 사용해야할 때 프로미스 객체를 리턴하게 만들어서 사용하면 callbaeck hell(콜백 중첩)을 방지할 수 있고 에러처리를 수월하게 할 수 있다.

- ### Classes(클래스)

class를 만들려면 `class`  뒤에 두 개의 중괄호가 있는 class 이름을 사용한다.

```jsx
class Person {
	constructor() {

	}
}
```

 `new` 객체를 사용하여 `class` 메서드와 속성에 액세스할 수 있다.

```jsx
class Person {
	constructor(name, age) {
		this.name = name;
		this.age = age;
	}
}

const user = new Person('lemming', 20);

console.log(user.name); // lemming
console.log(user.age); // 20
```

다른 class에서 상속하려면 `extends` 키워드 다음에 상속할 class의 이름을 사용합니다.

```jsx
class Person {
	constructor(name, age) {
		this.name = name;
		this.age = age;
	}

	introduce() {
		console.log(`안녕하세요 ${this.name}입니다. 나이는 ${this.age}살입니다.`);
	}
}

// Person 메서드 및 속성 상속
class UserProfile extends Person {
	userName() {
		console.log(this.name);
	}
}

const profile = new UserProfile('lemming', 20);

profile.introduce(); // 안녕하세요 lemming입니다. 나이는 20살입니다.
profile.userName(); // lemming
```
## json-server의 이해
