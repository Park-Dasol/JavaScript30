# Javascript30 - Day05

> Flex Panels Image Gallery





## CSS selectors

[W3schools CSS selectors](https://www.w3schools.com/cssref/css_selectors.asp)

| Selector      | Example        | Description                   |
| ------------- | -------------- | ----------------------------- |
| ` `              | div  p       | 자손 <p> 전부       |
| >             | div > p        | 자식 <p> 전부                 |
| *             | div > *        | 모든 자식 태그                |
| :first-child  | p:first-child  | 자식태그 중 첫번째 자식인 <p> |
| :nth-child(n) | p:nth-child(2) | 자식태그 중 n번째 자식인 <p>  |



## nth-child vs. nth-of-type

- nth-child : **p : nth-child(n)** 이런식으로 사용하고, n번째 자식이 p일 경우에 적용된다. n번째 자식이 p태그가 아니면 적용되지 않는다.
- nth-of-type: **p:nth-of-type(n)** 이런식으로 사용하고, p태그중에서 n번째인 태그에 적용된다.



## 자손선택자 vs. 자식선택자

[w3schools css combinators](https://www.w3schools.com/css/css_combinators.asp)

- 자손선택자( ) : 특정 요소의 하위에 있는 모든 자손을 선택한다.
- 자식선택자(>) : 특정 요소의 자식들만 선택한다.
