---
description: 이번주 단어가 많네.
---

# 학습 키워드

Express 란 ([Express](https://expressjs.com/ko/))

Node.js를 위한 빠르고 개방적인 간결한 웹 프레임워크

\->Node.js는 Chrome의 V8엔진을 이용하여 JavaScript로 브라우저가 아니라 서버를 구축하고, 서버에서 JavaScript가 작동되도록 해주는 런타임 환경(플랫폼)이라는 군,,

\->Express는 Node.js를 사용하여 쉽게 서버를 구성할 수 있게 만든 클래스와 라이브러리의 집합체

\->가장 많이 쓴단다.&#x20;



URL 구조

웹에서 HTML 페이지, CSS 문서, 이미지 등 리소스의 위치를 나타내는 주소를 뜻한다.

흔히 웹 사이트 주소로 알고 있지만, URL은 웹 사이트 주소뿐만 아니라 컴퓨터 네트워크상의 자원을 모두 나타낼 수 있다.

{% embed url="https://developer.mozilla.org/ko/docs/Learn/Common_questions/Web_mechanics/What_is_a_URL" %}

REST API

이거 지난주에도 한거 같은데,,



HTTP Method(CRUD)

Create, Read, Update, Delete

백과 프런트는 URL로 소통함. 그때사용 함.



Fetch API 란

JavaScript에서 서버로 네트워크 요청을 보내고 응답을 받을 수 잇도록 해주는 메서드.

예전에 Ajax로 쓰던거구나..

```jsx
fetch(url, options)
  .then((response) => console.log("response:", response))
  .catch((error) => console.log("error:", error));
```



Promise

ㅂ

비동기 처리 상태와 처리 결과를 관리하는 객체

sync/await 역할인가?



ReadableStream

JavaScript에서 데이터를 한번에 처리하지 않고 stream 방식으로 처리하는 인터페이스

```javascript
const readableStream = new ReadableStream({
    start(controller) {

    },
    pull(controller) {

    },
    cancel(reason) {

    }
});
```



Unicode

유니코드가 유니코드지,,

숫자와 글자, 즉 키와 값이 1:1로 매핑된 형태의 코드

아스키코드에서 0x41=A로 매핑된 것처럼, ASCII로 표현할 수 없는 문자들을 유니코드라는 이름으로 전 세계의 모든 문자(값)를 특정 숫자(키)와 1:1로 패밍한 것.

{% embed url="https://ko.wikipedia.org/wiki/%EC%9C%A0%EB%8B%88%EC%BD%94%EB%93%9C_%EC%98%81%EC%97%AD" %}
유니코드 블럭
{% endembed %}

UTF-8 대체로 효율적이라 세계적으로 많이 쓴다.



CORS 란

서버가 다른 출처로부터 액세스를 허용하거나 제한할 수 있게 하는 HTTP 헤더 기반의 메커니즘

출처: Protocol, Host, Port 까지

[https://evan-moon.github.io/2020/05/21/about-cors/](https://evan-moon.github.io/2020/05/21/about-cors/)



React Hook 이란

함수형 컴포넌트에서 다양한 작업을 할 수 있게 해주는 라이브러리

많이 사용하는 류의 함수를 제공해주는 것 같다.



useState

가장 기본적인 hook으로, 상태를 관리 한다.

현재 상태를 나타내는 state값(count)과 이 상태를 변경하는 setState(setCount) 한 상으로 제공.

const \[ count, setCount ] = useState(0);



useEffect

렌더링에 맞춰서 사용하는 듯 하다.

\-페이지가 렌더링 될 때마다 데이터를 불러온다.

```
React.useEffect(() => {
  dispatch(getActions.getFundingAC(page));
});
```

\-첫 렌더링 시에만 함수를 실행한다.(의존성 배열에 빈배열)

```
React.useEffect(() => {
  dispatch(getActions.getFundingAC(page));
}, []);
```

\-의존성 배열에 넣어준 값이 변할 때마다 함수 실행

```
const [page, setPage] = React.useState(1)

React.useEffect(() => {
  dispatch(getActions.getFundingAC(page));
}, [page]);
```



useContext

context를이용하면명시적으로 props를 넘겨주지 않아도 값을 공유할 수 있게 해준단다.

useContext를 context를 더 쉽게 사용할 수 있게 해주겄지,,



useRef

특정 DOM에 접근하여 DOM조작을 가능하게 한다.

렌더링과는 무관하게 값이 유지되어야 할 때 사용. 주로 DOM요소나 외부 라이브러리의 인스턴스와 같이 렌더링과는 직접적으로 관련이 없는 값들을 저장할 때 사용



useLayoutEffect

DOM이 그려지기 이전 시점에 동기적으로 수행된다. 즉 컴포넌트들이 render 된 후 실행되며, 그 이후에 paint 된다. paint가 되기 전에 실행되기 때문에 DOM을 조작하는 코드가 존재하더라도 사용자는 깜빡임을 경험하지 않는다.



React StrictMode 란

애플리케이션의 잠재적인 문제를 알아내기 위한 도구.&#x20;



Hook의 규칙

1.최상위에서만 Hook을 호출.

반복문, 조건문, 중첩된 함수내에서 Hook 호출하면 안 됨.

2.React 함수 내에서 Hook을 호출

일반적인 js 함수에서는 호출하면 안 된다.



usehooks-ts

사용하기 좋은 함수들 제공하는 라이브러리인듯 함.



useBoolean

참/거짓을 다룰 때&#x20;



useEffectOnce

의존성 배열 빈 배열로 넣어서 useEffect 만들었던 것, useEffectOnce로 하면 됨.



useFetch

fetch가 간단해진다.



useInterval

setTimeout같은 거.&#x20;



useEventListener

eventListener 쉽게 구현해주는 건가보다.



useLocalStorage

storage 쉽게 사용할 수 있게 해주는 거겠지,,



useDarkMode

OS에 다크모드가 있나부다.



swr

이것도 라이브러리란다. 리액트에 뭐가 많네.

SWR을 사용하면 간편하게 데이터를 가져오고, 캐시하여 이전 데이터를 재사용하며, 신선한(?) 데이터를 가져와서 사용자 경험을 향상할 수 있다고 한다.

영어로 뭐라고 되있길래 "신선한"으로 번역한걸까,,



react-query

이것도 라이브러리란다.&#x20;

애플리케이션의 데이터를 관리하고 동기화하는데 사용된단다.







키워드를 검색하면서 느끼는 건데,,

예전엔 정보가 많지 않은 대신, 존재하는 정보는 양질의 것이었는데,,

요즘은 무조건 블로그에 글을 쓰고 보는 걸까,

학교에서 블로그에 글 쓰기로 점수를주는 건가,,



