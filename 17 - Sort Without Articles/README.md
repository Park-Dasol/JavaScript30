

# 정규 표현식

[정규표현식 공식문서](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/%EC%A0%95%EA%B7%9C%EC%8B%9D)

> `//`로 감싸는 패턴

```
bandName.replace(/^(a |the |an )/i, "").trim()
```



## 특수문자



- `\` : 
  - 특수문자가 아닌문자 앞에서 : 해당 문자는 특별하고 문자 그대로 해석하면 안된다는 사실을 가리킴, **특별한 단어 경계 문자**를 형성
  - 특수문자 앞에서 : 다음에 나오는 문자는 특별하지 않고, 문자 그대로 해석되어야 한다는 사실을 가리킴
- `^` : 입력의 시작 부분에 대응
- `|` : 또는
- 





## 플래그



- `i ` :  대소문자 구분 없는 검색