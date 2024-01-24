# 코딩 테스트 readline 사용법

```js
const readline = require('readline');
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

rl.on('line', function (line) {

  // 입력 받은 값을 처리하는 코드
  // close가 없으면 무한하게 입력 받으니 주의
  rl. close();

}).on('close',function(){

  // 입력이 끝나고 실행하는 코드
  process.exit();
});
```

# 1. 문자열 출력하기
* 문자열 str이 주어질 때, str을 출력하는 코드를 작성해 보세요.


```js
const readline = require('readline');
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

let input = [];

rl.on('line', function (line) {
    input = [line];
}).on('close',function(){
    str = input[0];

    // 그냥 콘솔로 찍어봄, 통과
    console.log(str);
});
```
