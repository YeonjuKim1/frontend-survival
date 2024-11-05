# 학습 키워드

1.REST API 란 무엇인가?

REST를 기반으로 만들어진 API.

REST란,

\-HTTP URI를 통해 자원(Resource)을 명시하고,

\-HTTP Method(POST, GET, PUT, DELETE, PATCH 등)를 통해

\-해당 자원(URI)에 대한 CRUD Operation을 적용하는 것을 의미.



2.GraphQL 란 무엇인가?

API를 위한 Query Language이며 타입 시스템을 사용하여 쿼리를 실행하는 서버사이드 런타임. GraphQL은 특정한 데이터베이스나 특정한 스토리지 엔진과 관계되어 있지 않으며 기존 코드와 데이터에 의해 대체.

SQL이 데이터베이스 시스템으로부터 데이터를 가져오는 목적을 가진다면, GraphQL은 클라이언트가 데이터를 서버로부터 가져오는 것을 목적으로 한다.



3.GraphQL은 왜 등장했는가?

REST API가 자원을 효율적으로 주고 받는 방식에 대한 고민에서 고안된 것이라면,

GrapthQL은 화면구현을 더 잘하고자하는 고민에서 시작.

REST API쓰다가 불편하니까 만들었겠지...

\=> 장단이 있으니, 알맞게 잘 골라 쓰자.



4.REST API vs GraphQL

\-GraphQL은 보통 하나의 엔드포인트를 가진다.

\-GraphQL은 요청할 떄 사용하는 쿼리에 따라 다른 응답을 받을 수 있다.

\-GraphQL은 원하는 데이터(response)만 받을 수 있다.

[https://hahahoho5915.tistory.com/63](https://hahahoho5915.tistory.com/63)



5.JSON

Javascript 객체 문법으로 구조화된 데이터를 표현하기 위한 문자 기반의 표준 포맷.

key와 value로 이루어져 있고, 데이터 교환 표준.

JSON.stringify(arg)

JSON.parse(arg)



6.DSL(Domain-Specific Language) : 도메인 특화 언어

반대: General Purpose Language

비슷한 도메인에서 많 쓰이는 개발 패턴 같은 느낌..



7.선언형 프로그래밍

'무엇을' 할 것인가에 관한 것

SQL, HTML + JavaScript, C#, Python



8.명령형 프로그래밍

'어떻게' 할 것인가에 관한 것

C,C++,Java + JavaScript, C#, Python



9.SRP(단일 책임 원칙)

하나의 객체(클래스)는 하나의 기능을 담당하여 하나의 책임을 수행해야한다는 의미.



10.Atomic Design

작은 단위의 컴포넌트를 재사용성이 강하고, 단단하게 잘 설계함으로써 지속적으로 개발하기 용이하게 하는 방식.

더 이상 쪼갤 수 없을때까지 쪼개라는 의미인 듯.



11.React component 와 props

이랙트는 컴포넌트 기반 구조이고, props는 컴포넌트의 속성

{% embed url="https://ko.legacy.reactjs.org/docs/components-and-props.html" %}

12.React state란?

리액트 컴포넌트의 변경 가능한 데이터

setState



13.DRY 원칙

소프트웨어 개발 3대 원칙

\-KISS(Keep It Simple Stupid):간단하고 단순하게 만들어라.

\-YAGNI(You Ain't Gonna Need it):필요한 작업만 해라.

\-DRY(Do not Repeat Yourself):반복하지 마라.



14.SSOT(Single Source of Truth): 단일 진실 공급원

정보 모형과 관련된 데이터 스키마의 모든 데이터 요소를 한 곳에서만 제어 또는 편집하도록 조직하는 관례

데이터 무결성, 신뢰성, 일관성을 강화하는데 도움을 주는 핵심 원칙



15.useState

리액트의 상태 관리 기능 중 하나. 컴포넌트에서 동적인 데이터를 다룰 때 사용.

useState는 컴포넌트에 state 변수를 추가할 수 있게 해주는 React 훅입니다.

const \[state, setState] = useState(initialState)



16.1급 객체(first-class object)란?

다른 객체들에 일반적으로 적용 가능한 연산을 모두 지원하는 객체

\-변수에 할당할 수 있다.

\-다른 함수를 인자로 전달 받는다.

\-다른 함수의 결과로서 리턴될 수 있다.



17.Lifting State Up: 상태 끌어 올리기

2개 이상의 자식 컴포넌트가 동일한 데이터를 공유해야 할 때 사용. 공유되는 상태를 가장 가까운 공통 부모 컴포넌트로 끌어올림.

\->상위 컴포넌트의 "상태를 변경하는 함수" 그 자체를 하위 컴포넌트로 전달하고, 이 함수를 하위 컴포넌트가 실행하게 만듦.







