# html5 css3 practice

## html tag

- lang 속성

```html
<html lang="ko"></html>
```

실제 웹 브라우저 동작하는 데 어떠한 영향도 끼치지 않음. 검색 엔진이 탐색할 때 어떠한 언어로 만들어져있는지 인식할 때 참조.

- doctype

```html
<!-- HTML5 -->
<!DOCTYPE html>

<!-- HTML4 Frameset -->
<!-- 프레임셋을 구현하기 위해서 사용한다. -->
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "http://www.w3.org/TR/xhtml1-frameset.dtd">

<!-- HTML4 Strict -->
<!-- W3C가 의도했던 문서 타입으로, 구조와 표현을 분리하기 위해 단계적으로 사라질 표현에 관한 요소와 속성을 배제한 문서 타입이다. center, font, iframe, strike, u, 새창띄우기 등이 제한된다. -->
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1-strict.dtd">

<!-- HTML4 Traditional -->
<!-- 기존에 만들어진 문서들과의 호환성을 유지하기 위해 사용한다. iframe과 새창띄우기(target="_blank")등을 사용할 수 있어 XHTML 사용시 이것을 추천한다. -->
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1-transitional.dtd">
```

## block 형식의 태그와 inline 형식의 태그

### inline vs inline-block

#### inline

- width, height 속성 적용 안됨
- margin 좌우만 적용

#### inline-block, block

- width, height, margin 모두 적용 가능

### block

- div
- h1 ~ h2
- p
- 목록 태그
- 테이블 태그
- form 태그

### inline

- span
- a
- input
- 글자 형식

### inline-block

- 이미지 태그
- 멀티미디어 태그

## 시멘틱 구조 태그

- header
- nav
- aside
- section
- article
- footer

div 와 같은 기능, 검색 엔진에서 쉽게 이해할 수 있게 하는 데 의미가 있음

## css 선택자

http://www.nextree.co.kr/p8468/

- 일반 구조 선택자

  - :first-child
  - :last-child
  - :nth-child(수열)

- 형태 구조 선택자

  - :first-of-type
  - :last-of-type
  - :nth-of-type(수열)

- 시작 문자 선택자

  - ::first-letter
  - ::first-line

- 전후 문자 선택자
  - ::after
  - ::before

### 주의 사항

1. 후손 선택자

```css
#header h1,
h2 {
  color: red;
}
/* header h1 과 일반 h2 가 선택 됨 */
/* h1, h2 모두 후손 선택자를 선택하려면 아래와 같이 사용 */
#header h1,
#header h2 {
  color: red;
}
```

2. 자손 선택자

- table 일 경우 tbody 가 자동으로 추가하므로 자손 선택자를 table 에 사용 하지 않아야 함.

## css 속성

### 크기 단위

- % : 백분율 단위
- em : 배수 단위
- px : 픽셀

```css
p:nth-child(1) {
}
p:nth-child(2) {
  font-size: 100%;
}
p:nth-child(3) {
  font-size: 150%;
}
p:nth-child(4) {
  font-size: 200%;
}

p:nth-child(1) {
}
p:nth-child(2) {
  font-size: 1em;
}
p:nth-child(3) {
  font-size: 1.5em;
}
p:nth-child(4) {
  font-size: 2em;
}

p:nth-child(1) {
}
p:nth-child(2) {
  font-size: 16px;
}
p:nth-child(3) {
  font-size: 24px;
}
p:nth-child(4) {
  font-size: 32px;
}
```

모두 같은 결과

### 색상 단위

| 단위 형태                               | 설명           |
| --------------------------------------- | -------------- |
| #000000                                 | HEX 코드 단위  |
| rgb(red, green, blue)                   | RGB 색상 단위  |
| rgba(red, green, blue, alpha)           | RGBA 색상 단위 |
| hsl(hue, saturation, lightness)         | HSL 색상 단위  |
| hsla(hue, saturation, lightness, alpha) | HSLA 색상 단위 |

- alpha 값은 투명도를 의미 0.0부터 1.0 사이의 숫자 입력
