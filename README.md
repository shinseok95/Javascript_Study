# Javascript-Study
> 자바스크립트 기초 문법 정리
  
## 기초

### 변수 할당

const : 상수 선언<br>
let : 변수 선언<br>
<br>

### 문자열

"" , '' : 단순 문자열<br>
`` : 표현식 가능 문자열 (ex : const message = `나는 ${30+1}살 입니다.`)<br>
<br>

### typeof 연산자

```javascript

const name = 'mike'
console.log(typeof name) // String 출력
```
<br>

### alert, prompt, confirm

alert : 메시지를 보여주는 창<br>
prompt : 값을 입력받는 창 (문자열 입력)<br>
confirm : 확인을 받는 창<br>

<br>

### 형변환(명시적 형변환)

String(X) :  X -> 문자열<br>
Number(X) : X -> 숫자형 (X에 글자가 들어가면 NaN 반환)<br>

Number(null) -> 0 <br>
Number(undefined) -> NaN<br><br>

Boolean(X) : X -> boolean형 (0,‘’, null, undefined, NaN -> false / 그 외 -> true)<br>
<br>

### 비교 연산자

== (동등 연산자) : 두 값이 같은지 비교<br>
=== (일치 연산자) : 두 값과 타입까지 비교<br>
<br>

### function

function(name = ‘friend’){} -> 매개변수 default 값<br>
return이 없어도 undefined를 반환<br>
<br>

### 함수 표현식

코드에 도달하면 생성<br>

```javascript

let sayHello = function(){}
sayHello();
```
<br>

### 화살표 함수

```javascript

let sayHello = (name) => {
 const msg = `Hello, ${name}`;
 console.log(msg);
}

let add = (num1, num2) => num1 + num2;
```
<br>

### 호이스팅(hoisting)

초기화 단계에서 모든 함수의 선언문을 생성 -> 어디서든 호출 가능
<br>

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
<br>

접근 : superman.name / superman[‘age’]<br>
추가 : superman.gender = ‘male’ / superman[‘hairColor’] = ‘black’<br>
삭제 : delete superman.hairColor;<br>
<br>

```javascript

// user에 age가 있는지 확인 (true, false)

if (‘age’ in user){

}
```
<br>

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
<br>

## 참고 사이트

> 기초

https://www.youtube.com/watch?v=KF6t61yuPCY <br>

> 기본
https://www.youtube.com/watch?v=4_WLS9Lj6n4 <br>
