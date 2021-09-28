### 의도를 분명히 밝혀라

| X | O |
|---|---|
|int d|int elapsedTimeInDays| 
| |int daysSinceCreation|
| |int daysSinceModification|
| | int fileAgeInDays|


- 수행 기능, 사용 방법 등이 변수 명에 나타나야한다.

### 그릇된 정보를 피하라

`Set<Account> accountList;`

### 의미있게 구분하라

- Info, Data 등은 불용어에 속한다. 
    * ex) Customer 클래스와 CustomerObject 클래스가 있다면 급여는 어느 클래스를 참고해야할까? -> 모륾

### 발음하기 쉬운 이름을 사용하라

- Date genymdhms; -> Date generationTimestamp;

### 검색하기 쉬운 이름을 사용하라

- 숫자, e, t 등은 지양

### 인코딩을 피하라

- 예를 들면 헝가리식 표기법 등 변수명 설정에 법칙을 만드는 것

- 인터페이스 클래스에는 접두어 X, 대신 구현 클래스에는 Impl 등과 같이 접미어 가능

### 자신의 기억력을 자랑하지 마라

- 문자 하나만 사용하는 변수 명은 문제(루프에서 반복 횟수를 세는 i,j,k 는 괜찮, l 은 안됨!! l 까지 가는 반복문 X)

- 명료함이 최고, 남들이 이해하는 코드를 작성

#### 클래스 이름

- 명사나 명사구

- Customer, WikiPage, Account, AddressParser 등은 Good
- Manager, Processor, Data, Info 등은 지양 

#### 메소드 이름

- 동사나 동사구

- 접근자(Accessor), 변경자(Mutator), 조건자(Predicate) 는 자바빈 표준에 따라 get, set, is 를 붙인다.

- 생성자를 overloading(중복정의) 할 때는 정적 팩토리 메소드를 사용한다.

### 한 개념에 한 단어를 사용하라

- 추상적인 개념 하나에 단어 하나를 매핑하고 이를 고수한다.

- fetch, retrieve, get 등 비슷한 어휘를 같은 개념에 사용 X, 일관성 있는 어휘 사용

- controller, manager, driver 도 마찬가지이다.

### 한 단어를 두 개념에 사용하지 마라

- add 의 개념과 append 의 개념은 다르다.

### Solution Domain(해법 영역?) 과 Problem Domain(문제 영역?) 이름을 사용하라

- 이 부분 더 공부하기

### 의미있는 맥락을 추가하라

- firstName, lastName, street, city, state 라는 변수 목록이 있으면 state 가 "주" 라는 것을 알지만 state 만 따로 보면 "주" 라는 것을 알기 힘들다.

- addrCity, addrState 처럼 접두어를 추가하거나 Address 라는 클래스 안에 넣는 것이 적절하다.

