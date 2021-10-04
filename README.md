# Javascript-Study
> 자바스크립트 기초 문법 정리
  
## 기초

### 변수 할당

const : 상수 선언
let : 변수 선언
 
### 문자열

"" , '' : 단순 문자열
`` : 표현식 가능 문자열 (ex : const message = `나는 ${30+1}살 입니다.`)

### typeof 연산자

```javascript

const name = 'mike'
console.log(typeof name) // String 출력
```

### alert, prompt, confirm

alert : 메시지를 보여주는 창
prompt : 값을 입력받는 창 (문자열 입력)
confirm : 확인을 받는 창

### 형변환(명시적 형변환)

String(X) :  X -> 문자열
Number(X) : X -> 숫자형 (X에 글자가 들어가면 NaN 반환)

Number(null) -> 0
Number(undefined) -> NaN

Boolean(X) : X -> boolean형 (0,‘’, null, undefined, NaN -> false / 그 외 -> true)

### 비교 연산자

== (동등 연산자) : 두 값이 같은지 비교
=== (일치 연산자) : 두 값과 타입까지 비교

### function

function(name = ‘friend’){} -> 매개변수 default 값
return이 없어도 undefined를 반환

### 함수 표현식

코드에 도달하면 생성

```javascript

let sayHello = function(){}
sayHello();
```

### 화살표 함수

```javascript

let sayHello = (name) => {
 const msg = `Hello, ${name}`;
 console.log(msg);
}

let add = (num1, num2) => num1 + num2;
```

### 호이스팅(hoisting)

초기화 단계에서 모든 함수의 선언문을 생성 -> 어디서든 호출 가능

### Object

```javascript

let sayHello = function(){}
const superman = {
 name : ‘clark’,
 age : 33,
 fly(){
  console.log(‘날아갑니다.’) 
 }
}
```

접근 : superman.name / superman[‘age’]
추가 : superman.gender = ‘male’ / superman[‘hairColor’] = ‘black’
삭제 : delete superman.hairColor;

```javascript

// user에 age가 있는지 확인 (true, false)

if (‘age’ in user){

}
```

### Array

```javascript

students.length // 배열 길이 반환

student.push(X) // 배열 끝에 요소 추가
student.pop(X) // 배열 끝 요소 제거

student.unshift(X) // 배열 앞에 요소 추가
student.shift(X) // 배열 앞에 요소 제거

// index for문
for (let index = 0 ; index < days.length; index++){
 console.log(days[index])
}

// 
for (let day of days){
 console.log(day)
}
```


## 참고 사이트

> 기초

https://www.youtube.com/watch?v=KF6t61yuPCY <br>

> 기본
https://www.youtube.com/watch?v=4_WLS9Lj6n4 <br>
