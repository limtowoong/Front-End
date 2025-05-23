# 📚 JavaScript 기초 - prompt 사용법

## 🧠 prompt란?

`prompt()`는 브라우저에서 사용자에게 입력을 받을 수 있게 해주는 **팝업 입력창 함수**입니다.

```js
const name = prompt("너의 이름은?"); #입력: james
alert(`안녕, ${name}!`); #출력: 안녕, james
```

```js
const a = prompt("첫 번째 숫자:"); #입력: 1
const b = prompt("두 번째 숫자:"); #입력: 2
const sum = Number(a) + Number(b);
alert(`합계는 ${sum}입니다.`); #출력: 합계는 3입니다.
```