# Js-output-based-questions
This repo contains most asked javascript output-based questions

1. Question
```   
var num = 8;
var num = 10;
console.log(num);

Answer: 10
```

2. Question
```
function sayHi() {
  console.log(name);
  console.log(age);
  var name = 'Ayush';
  let age = 21;
}

sayHi();

Answer: undefined and ReferenceError 
```

3. Question
```
function getAge() {
  'use strict';
  age = 21;
  console.log(age);
}

getAge();

Answer: Reference error
```

4. Question
```
+true;
!'Ayush';

Answer: 1 and false
```

5. Question
```
let number = 0;
console.log(number++);
console.log(++number);
console.log(number);

Answer 0 2 2. Explanation The postfix unary operator ++:
```

6. Question
```
function sum(a, b) {
  return a + b;
}

sum(1, '2');

Answer: '12'
```

 7. Question
```
typeof [];

Answer: Object
```
8. What's the output?
```
for (var i = 0; i < 3; i++) {
  setTimeout(() => console.log(i), 1);
}

for (let i = 0; i < 3; i++) {
  setTimeout(() => console.log(i), 1);
}

Answer: 3 3 3 and 0 1 2 (var will create variable which is global to function as let will create new variable for every loop)
```
