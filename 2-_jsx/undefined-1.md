# 과제

git에서 fork 받았는데, 명령어들이 실행되지 않는다.&#x20;



1.parcel을 찾을 수 없단다.

package.json에 다 리스트업 되어 있는데, maven reload처럼 설치를 해줘야 하는 걸까?

\>npm i

package.json에 명시되어 있는 모든 의존 패키지들을 설치해서 node\_modules에 적재해 준단다.

\>npm ci

package-lock.json 에 명시되어있는 정확한 버전의 패키지들을 설치해서 node\_modules에 적재해 준단다.

npm i 와는 다르게 절대 package-lock.json을 수정하지 않는다고 한다.



2.Expected linebreaks to be 'LF' but found 'CRLF'.

윈도우 운영체제는 CR+LF(\r\n)&#x20;

유닉스 계열은 LF(\n)

나는 윈도우를 쓴다. 맥북은 써본적도 없다. 폰도 안드로이드만 쓴다. 그래서 진정한 개발자가 아니다.

eslintrc.js rules에 'linebreak-style': \['error', 'windows'],를 추가하면, 설정 파일들에서 Expected linebreaks to be 'CRLF' but found 'LF'. 이 에러가 발생하고, 추가하지 않으면 Expected linebreaks to be 'LF' but found 'CRLF'. 에러가 발생한다. 파일을 여러 환경에서 생성했나보다.

vscode에서 변경하는 걸 찾다가, 그냥 설정을 'linebreak-style': 0, 이렇게 바꿔버렸다.





3.Module './App' was resolved to 'D:/Anne/front-survival/frontend-survival-week02/src/App.tsx', but '--jsx' is not set.

음,,,,

JSX가 들어간 문법은 .ts가 아니라, .tsx 라고 해줘야 한다.라고 하네.









