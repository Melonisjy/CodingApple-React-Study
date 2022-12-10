## 2022 코딩애플 리액트 강의 정리

### 2강 정리
원래 리액트에서 div 태그 만드는 법
- React.createElement('div', null, 'Hello World")
<br>

html에 변수를 넣고 싶을 땐(= 데이터바인딩) '{}'<br>
ex)
``` 
let post = "강남 우동 맛집";
...
<h4>{ post }</h4>
```

style 넣을 땐 style={{style name: 'value'}}
<hr>

### 3강 정리
return () 안에는 병렬로 2개 이상의 태그 금지<br>
ex)
```
<div className="App"> //이런식의 2개 이상의 병렬 태그 금지
</div>
<div></div>
```  

state 만드는 법
1. import { useState }
2. useState(보관할 자료)
3. let [작명1, 작명2] - 작명1: state에 보관했던 자료 / 작명2: state 변경을 도와주는 함수

(참고)Destructuring 문법
```
let num = [1,2]; // <- array

let a = num[0]; // 1을 뽑음.
let c = num[1]; // 2를 뽑음.

let [a, c] = [1,2]; // Destructuring 문법
```

state 쓰는 이유
- state를 쓰던 html은 자동으로 재렌더링됨.
- 하지만 다 변수대신 state를 쓰기 보다는 자주 변경되는 사항에 대해서만 state를 쓰는 것이 좋다.
<hr>

### 3강 정리

warning message 끄는 법 <br>
```
/* eslint-disable */
```
<hr>

### 4강 정리
<hr>

### 5강 정리

(참고) array또는 object를 다룰 때는 원본은 보존하는 것이 좋다. <br>

#### state 동작 원리
[state 변경함수의 특징] <br>
기존 state == 신규 state 면 변경을 안해준다. <br>
[array/object 특징] <br>
array/object를 담은 변수에는 화살표만 저장이 된다. <br>
[...변수] = ...은 괄호를 벗긴다는 의미. 새로 독립적인 array가 생성이 된다. <br>
<hr>

### 6강 정리

컴포넌트 만드는 문법 1
1. function 만들기. (function 바깥에 만들어야 함 & 첫글자는 대문자)
2. return()안에 html 담기
3. <함수명><함수명/> 쓰기


(참고 1)의미없는 div 대신 <></> 사용 가능 <br>
(참고 2)<함수명></함수명>, <함수명/> 둘 다 가능 <br>

어떤 것을 컴포넌트로 만들면 좋을까?
1. 반복적인 html 축약할 때
2. 큰 페이지들
3. 자주 변경되는 것들 

컴포넌트의 단점
1. state를 가져다쓸 때 문제가 생긴다.

(참고 3)컴포넌트 만드는 문법 2 <br>
```
const Modal = () => {}
```


