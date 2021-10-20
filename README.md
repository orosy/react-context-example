# Context API

### 하위 컴포넌트 전체에 데이터를 공유하는 법 <br>
- 데이터를 Set 하는 법
    - 가장 상위 컴포넌트 ⇒ 프로바이더
- 데이터를 Get 하는 법
    - 모든 하위 컴포넌트에서 접근 가능
        - 컨슈머로 하는 방법
        - 클래스 컴포넌트의 `this.context`로 하는 방법
        - 함수 컴포넌트의 `useContext`로 하는 방법

### 데이터를 Set 하기 <br>
1. 컨텍스트를 생성한다.
2. 컨텍스트, 프로바이더를 사용한다.
3. value를 사용

### 데이터를 Get 하기 (1) - Consumer <br>
1. 컨텍스트를 가져온다.
2. 컨텍스트, 컨슈머를 사용한다.
3. value를 사용

### 데이터를 Get 하기 (2) - class <br>
1. static contextType 에 컨텍스트를 설정한다.
2. this.context ⇒ value 이다.
3. 단점: 여러 개를 지정할 수 없음
