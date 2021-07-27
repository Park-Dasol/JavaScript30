# Javascript30 - Day02

> CSS + JS Clock







## Date()

[Javascript MDN Date()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)

```javascript
const date = new Date(); # returns a new Date object
const [month, day, year]       = [date.getMonth(), date.getDate(), date.getFullYear()];
const [hour, minutes, seconds] = [date.getHours(), date.getMinutes(), date.getSeconds()];
```



## SetInterval

[Javascript MDN setInterval()](https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/setInterval)

> 함수를 반복적으로 수행하거나 호출할때, 매번 호출시마다 일정 시간을 연기하는 메소드

- 각 인터벌 고유의 인터벌 Id를 가지고 있어서 **clearInterval()** 메소드를 호출함으로써 제거할 수 있다.
- delay 의 단위는 milliseconds
- setInterval을 제거하기 위해 clearInterval을 사용하고, setTimeout을 제거하기 위해 celarTimeout을 사용한다.

```javascript
var intervalID = setInterval(func, [delay, arg1, arg2, ...]);
var intervalID = setInterval(function[, delay]);
var intervalID = setInterval(code, [delay]);
```



## transform : rotate(deg)

[CSS MDN trnasform](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)

> CSS의 transform 프로퍼티는 회전, 크기변경, skew(찌그러트리기), trnaslate(위치변경)을 제공한다.

```
transform: rotate(45deg);
transform: rotate(3.1416rad);
transform: rotate(-50grad);
transform: rotate(1.75turn);
```

