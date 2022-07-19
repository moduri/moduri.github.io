---
layout: post
title:  "map, forEach"
date:   2022-07-19
categories: JS
---


- <h3>forEach는 반복문과 비슷하고, map은 요소값을 다른 새로운 배열을 생성하기 위한 고차함수다. </h3> 

<hr>

- <h3>map</h3>


```javascript
console.log('map');
let arr = [1, 1, 2, 2, 3, 3];
let arr2 = arr.map((value, idx) => value * idx);
console.log(arr2)
```

    map
    [ 0, 1, 4, 6, 12, 15 ]


<hr>


```javascript
let arr = ['1', '2', '3']
let arr2 = arr.map(str => Number(str));
console.log(typeof(arr2[1]))
```

    number


- map 메서드는 자신을 호출한 배열의 모든 요소를 순회하면서 인수로 전달받은 콜백 함수를 반복 호출한다
- 그리고 콜백 함수의 반환값들로 구성된 <b>새로운 배열</b>을 반환한다. 원본은 건들지 않는다.

<hr>

- <h3>forEach</h3>


```javascript
console.log('forEach')
let arr7 = [1, 2, 3, 4, 5]
arr6.map((arr) => arr * 2)
console.log(arr7)
```

    forEach
    [ 1, 2, 3, 4, 5 ]



```javascript
let numbers_arr = [1, 2, 3];
let my_list = [];
numbers_arr.forEach(x => my_list.push(x ** 2) );
console.log(my_list);
```

    [ 1, 4, 9 ]


- forEach 메서드는 내부에서 반복문을 통해 자신을 호출한 배열을 순회하면서 수행해야할 처리를 콜백 함수로 전달받아 반복 호출한다.
