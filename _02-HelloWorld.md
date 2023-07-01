## Hello, World!

### 1. Script 태그

```html
<!Doctype HTML>
<html>

    <body>

        <p>스크립트 전</p>

        <script>
            alert('Hello, world!);
        </script>

        <p>스크립트 후</p>

    </body>

</html>
```

- 웹 페이지에 자바스크립트 코드를 추가하기 위해 `<script>` 태그 사용
- `<script>` 태그에 자바스크립트 코드가 들어가고, 브라우저는 이 태그를 만나서 자동으로 처리함

    - type 속성: `<script type=…>`
    - language 속성: `<script language=…>`
    <br>필수 아님!


### 2. 외부 스크립트
- 자바스크립트 코드의 양이 많은 경우 파일로 소분 가능
- src 속성을 사용해 HTML에 삽입

```html
<script src="/path/to/script.js"></script>
```
- `/path/to/script.js` 는 사이트의 루트 ~ 파일이 위치한 절대경로를 나타냄 (현재 페이지에서의 상대경로 사용도 가능)


```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/lodash.js/4.17.11/lodash.js"></script>
```
- URL 전체를 속성으로 사용도 가능

---

- HTML 안에 직접 스크립트를 작성하는 방식은 스크립트가 아주 간단할 때만 추천
- 스크립트가 길어지면 분리된 파일로 만들어 저장하는 것을 권장함

---

- src 속성이 있으면 태그 내부의 코드는 무시됨
- `<script src="…">`로 외부 파일을 연결할지, `<script>` 태그 내에 코드를 작성할지를 선택해야 함