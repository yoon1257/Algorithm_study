# baekjoon 알고리즘 공부

개인 알고리즘 스터디 정리

### 파일을 불러와서 받는 법

📌 백준 node.js input 값 받아오기

```js
const readline = require("readline");
const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

const input = []; // 변수를 저장
rl.on("line", function (line) {
  // line이라는 변수를 입력
  input.push(line); // 1줄씩 입력받고 무한으로 입력받음
}).on("close", function () {
  // 컨트롤 + D를 누르면 종료됨. (백준에서는 입력끝나면 자동 종료)
  solution(input); // 원하는 함수 실행
  process.exit();
});
```
