## 변수와 상수

### 1. 변수
```javascript
let message;
```
- `let` 키워드를 사용해서 변수 선언
- `let` 대신 `var` 키워드를 사용할 수는 있지만 오래된 방식임

### 2. 상수
```javascript
const myBirthday = 18.03.2000;

myBirthday = 20.01.2000; // error
```
- 변하지 않는 변수를 선언할 때 `const` 사용
- 상수는 재할당할 수 없으므로 변경하려고 하면 에러 발생
