# Javascript30 - Day03

> Playing with CSS Variables and JS







## :root

> :root는 CSS의 슈도 클래스로 <html> 선택자와 같은 요소를 선택한다.

[CSS MDN :root](https://developer.mozilla.org/en-US/docs/Web/CSS/:root)



- 전역 CSS 변수 선언에 유용하게 사용할 수 있다.

```
# 사용
:root {
  --main-color: hotpink;
  --pane-padding: 5px 42px;
}
```





## setProperty()

> setProperty() 메소드는 CSS스타일 프로퍼티 값을 바꾸는데 사용한다.

[Javascript MDN setProperty](https://developer.mozilla.org/en-US/docs/Web/API/CSSStyleDeclaration/setProperty)



- propertyName은 변경할 CSS 프로퍼티 이름을 나타낸다.
- value(선택사항)는 새 프로퍼티의 값
- proority(선택사항)은 CSS의 important를 허용한다.
  - ex) "important", ""

```
# 사용
style.setProperty(propertyName, value, priority);
```





# document.documentElement

> document.documentElement는 document의 root 요소를 반환한다.
>
> 예를 들면, HTML documents의 <html> 요소

[Javascript MDN documentElement](https://developer.mozilla.org/en-US/docs/Web/API/Document/documentElement)



```
# 사용
const element = document.documentElement
```





- 종합하면, document.documentElement로 CSS에서 :root를 전역으로 선언해 놓았던 변수를 바꾸기 위해서 setProperty메소드를 이용한 것