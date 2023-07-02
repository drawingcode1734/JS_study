## 자료형
- 자바스크립트의 변수는 자료형에 관계없이 모든 데이터일 수 있음
    - 변수가 문자열이 될 수도, 숫자가 될 수도 있음
- 동적 타입(dynamical typed) : 자료의 타입은 있지만 변수에 저장되는 값의 타입은 언제든지 바꿀 수 있는 언어


### 1. 숫자형
- 숫자형 : 정수 및 부동소수점 숫자, 사칙연산 등을 할 수 있음
```javascript
let n = 5;
```
- 특수 숫자 값 `Infinity, -Infinity, NaN` 포함
    - 어느 숫자든 0으로 나누면 무한대 얻을 수 있음
    - 계산 중 에러 `NaN`


### 2. BigInt
- 길이 제약 없이 정수를 나타낼 수 있음
- 정수 리터럴 끝에 n 붙이면 만들기 가능


### 3. 문자형
- 문자열을 따옴표로 묶는데, 큰따옴표와 작은따옴표에 차이 없음
- 역따옴표로 변수나 표현식을 감싼 것 안에 `${ ... }` 를 넣어주면 변수나 표현식을 문자열 중간에 넣을 수 있음
```javascript
alert( `the result is ${1 + 2}` ); // the result is 3
```

### 4. 불린형
- true / false


### 5. 'null' 값
- `null` 값은 오직 `null` 값만 포함하는 별도의 자료형
- 다른 언어에서의 `null` 값과 성격이 다름 : 존재하지 않는 값, 비어있는, 알 수 없는 값
```javascript
let age = null;
```
- 나이를 알 수 없거나 그 값이 비어있다는 뜻


### 6. undefined
- 자신만의 자료형을 형성
- 값이 할당되지 않은 상태
- 변수는 선언했지만 값이 할당되지 않았으면 자동으로 변수에 `undefined` 값이 할당됨


### 7. 객체형
- 복잡한 데이터 구조를 표현할 때 사용, 이후 학습


### 8. 심볼형
- 객체의 고유한 식별자를 만들 때 사용


### 9. typedef
- 인수의 자료형을 반환함
    - 연산자 : typedef x
    - 함수 : typedef(x)

```javascript
typeof undefined // "undefined"

typeof 0 // "number"

typeof 10n // "bigint"

typeof true // "boolean"

typeof "foo" // "string"

typeof Symbol("id") // "symbol"

typeof Math // "object" → Math는 수학 연산을 제공하는 내장 객체

typeof null // "object" → 언어 자체의 오류이며 객체가 아님

typeof alert // "function" → 피연산자가 함수면 이렇게 반환하지만 사실 함수는 객체형임 (호환성 유지 위해서 남겨진 상태)
```