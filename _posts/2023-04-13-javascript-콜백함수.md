---
title: 콜백 함수
author: 
date: 2023-04-13 00:10:00 +0800
categories: [Study, Javascript]
tags: [Javascript]
render_with_liquid: false
---



## 콜백함수
함수는 하나의 자료형이기 때문에[그러니까 변수를 저장하는 데이터 형식(DATA Type)를 자료형이라고 하며, 함수가 호출될때 전달되는 매개변수는 데이터 형식을 가지고 있음] 매개변수로 전달할수 있다. 
매개변수를 전달하는 함수를 콜백함수(Callback function)이라 한다.

```javascript
 <script>

        function callThreeTimes(callback){
            for (let i = 0; i < 3; i++) {
                callback(i);
            }
        }
        //1
        function print(i){
            console.log(`${i}번째 호출입니다.`)
        }

        callThreeTimes(print);// 매개변수를 function print()를 던짐

        //2
        function callThreeTimes2(callback){
            for (let i = 1; i < 4; i++) {
                callback(i);
            }
        }

        callThreeTimes2(function(i){
          console.log(i);
        });

    </script>
```

위의 1번 코드의 경우 callThreeTimes 함수는  print 함수를 매개변수로 받아 함수(callback() )를 호출한다. callThreeTimes 함수 내부에서 callback(i)로 호출함 
2번 코드의 경우 callThreeTimes2 함수는 print 함수 대신 익명함수를 이용하여 함수를 호출함


## 콜백함수 대표적한 함수 

1. forEach()
function(value,index,array) //값,인덱스,배열(Array를 가지고 있는 함수이다.)


2. map()
map도 Array를 가지고 있는 함수로 콜백함수에서 리턴한 값들을 기반으로 새로운 배열을 만드는 함수

```javascript
let num =[1,2,3,4,5]

num = num.map(function(value,index,array) {
    return value *2;
})

num.forEach(console.log); // 매개변수로 console.log메소드 자체를 넘김 콜백함수는 ()를 제거한 채로 던저야함
```


3. fileter()
filter도 Array를 가지는 함수로 전체 배열에 조건을 명시하여 특정값을 가진 array를 구할때 사용하는것으로 보인다.


```javascript
const number = [1,2,3,4,5]

const evenNumber = number.filter(function(value,index){
    return value %2 == 0 // 조건을 명시
})//결과값은 0,2,4을 가진 배열을 가짐 

```

## 참고 
※ 화살표 함수 
콜백함수는 아니지만 콜백함수를 쉽게 입력하고자 사용되는 함수 생성방법으로 function키워드 대신 화살표 (=>)를 사용한다
```javascript
(매개변수)=>{

}

혹은

(매개변수)=>리턴값
```


