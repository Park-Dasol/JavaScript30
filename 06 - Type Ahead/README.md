

# Javascript30 - Day06

>  Ajax Type Ahead





## fetch()

> fetch()는 http 파이프라인을 구성하는 요소를 조작하는데 이용된다.

[Javascript MDN fetch()](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)





- fetch()사용시 응답을 포함하는 Response 객체를 반환한다.
- HTTP Response 이며, JSON 형태가 아니다.

- 사용예시

```javascript
fetch('http://example.com/movies.json')
  .then(blob => blob.json())
  .then(data => console.log(data))
```



## RegExp

> RegExp는 특정 텍스트의 패턴을 확인할 때 사용한다.

[Javscript MDN RegExp](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp)

- **리터럴표기법**과 **생성자**로 만들 수 있다.
- 리터럴표기법 : 정규 표현식 형태로 매칭을 비교, 정규 표현식이 변하지 않으면 리터럴 표기법을 사용
- 생성자 : 패턴이 변할 가능성이 있거나, 사용자 입력과 같이 알 수 없는 외부 소스에서 가져오는 정규 표현식의 경우 생성자 함수를 사용

```javascript
new RegExp(/ab+c/, 'i') // 리터럴
new RegExp('ab+c', 'i') // 생성자
```

- gi : global insensitive

- g 플래그가 포함되어 있으면, 일치하는 하위 문자열을 포함하는 `Array`를 반환한다.


