

## SPLICE

> splice() 메소드는 배열의 내용물을 제거/치환/삽입해서 변경하는 메소드



[MDN 설명 참고하기](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)



`splice(start, count, item)`

- start : 바꿀 배열의  인덱스
- count는 인덱스로부터 몇개의 요소를 변경할 것인지
- item을 비워두면 삭제, item이 있으면 삽입 혹은 치환이 된다.



## 삭제

- index 양수인 경우

```
const alphabet= ['A', 'B', 'C', 'D', 'E','F'] 
alphabet.splice(1, 1)
console.log(alphabet)

>> Array ["A", "C", "D", "E", "F"]
1번 인덱스의 요소가 삭제 되었다.
```

- index 음수인경우

```
const alphabet= ['A', 'B', 'C', 'D', 'E','F'] 
alphabet.splice(-1, 1)
console.log(alphabet)

>> Array ["A", "B", "C", "D", "E"]
인덱스가 음수인 경우 제일 마지막에 있는 요소부터 -1, -2,,, 이렇게 진행된다.
```





## 치환

```
const alphabet= ['A', 'B', 'C', 'D', 'E','F'] 
alphabet.splice(2, 4, 'Z')
console.log(alphabet)

>> Array ["A", "B", "Z"]
2번 인덱스부터 4개의 요소 대신 'Z'가 입력되었다.

const alphabet= ['A', 'B', 'C', 'D', 'E','F'] 
alphabet.splice(2, 10, 'Z')
console.log(alphabet)

>> Array ["A", "B", "Z"]
2번 인덱스부터 10개(배열의 남은 길이보다 큰 숫자가 입력되면 start부터 전부를 의미)
```





## 삽입

```
const alphabet= ['A', 'B', 'C', 'D', 'E','F'] 
alphabet.splice(2, 0, 'Z')
console.log(alphabet)

>> Array ["A", "B", "Z", "C", "D", "E", "F"]
2번 인덱스에 'Z'를 삽입
```

