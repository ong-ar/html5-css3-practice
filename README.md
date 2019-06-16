# html5 css3 practice

## html tag

- lang 속성
```html
<html lang="ko">
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