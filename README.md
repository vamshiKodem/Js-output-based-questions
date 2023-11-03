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

7.  Question

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

9. What's the output?

```
const shape = {
  radius: 10,
  diameter() {
    return this.radius * 2;
  },
  perimeter: () => 2 * Math.PI * this.radius,
};

console.log(shape.diameter());
console.log(shape.perimeter());

Answer: 20 and NaN (Arrow function refers to a global object whereas regular function will refer object to which is called)
```

10. What's the output?

```
let c = { greeting: 'Hey!' };
let d;

d = c;
c.greeting = 'Hello';
console.log(d.greeting);

Answer: Hello (As non-primitive type will assign reference when we assign to other variables)
```

11. What's the output?

```
let a = 3;
let b = new Number(3);
let c = 3;

console.log(a == b);
console.log(a === b);
console.log(b === c);

Answer: true, false, false
```

11. What's the output?

```
function Person(firstName, lastName) {
  this.firstName = firstName;
  this.lastName = lastName;
}

const member = new Person('Lydia', 'Hallie');
Person.getFullName = function() {
  return `${this.firstName} ${this.lastName}`;
};

console.log(member.getFullName());

Answer: TypeError ( If we use prototype it will work Person.prototype.getFullName = function() {
  return `${this.firstName} ${this.lastName}`;
};
```

12. What would be the output of the following code?

```
console.log(employeeId);
var employeeId = '19000';
Answer: undefined
```

13. What would be the output of following code?

```
var employeeId = '1234abe';
(function(){
	console.log(employeeId);
	var employeeId = '122345';
})();

Answer: undefined
```

14. What would be the output of following code?

```
(function() {
	console.log(typeof displayFunc);
	var displayFunc = function(){
		console.log("Hi I am inside displayFunc");
	}
}());

Answer: undefined
```

15. What would be the output of following code?

```
var employeeId = 'abc123';
function foo(){
	employeeId = '123bcd';
	return;
}
foo();
console.log(employeeId);

Answer: 123bcd
```

16. What would be the output of following code?

```
var employeeId = 'abc123';

function foo() {
	employeeId();
	return;

	function employeeId() {
		console.log(typeof employeeId);
	}
}
foo();

Answer: function
```

17. Return a new array with the user of id 2 change the city to new City

```
const data = [
  {
    id: 0,
    name: "my name",
    age: 22,
    address: [
      {
        city: "hyderabad",
        state: "telangana",
      },
    ],
  },
  {
    id: 1,
    name: "my name 2",
    age: 23,
    address: [
      {
        city: "hyderabad 2",
        state: "telangana 2",
      },
    ],
  },
  {
    id: 2,
    name: "my name 3",
    age: 22,
    address: [
      {
        city: "hyderabad 3",
        state: "telangana 3",
      },
    ],
  },
];

Answer:
const newData = data.map((data) => {
  if (data.id === 2) {
    return {
      ...data,
      address: [{ state: data.address[0].state, city: "my new City" }],
    };
  }
  return data;
});

```

18. What would be the output of following code?

```
 const outerFunction = () => {
    let b = 100;
    const innerFunction = () => {
      console.log(b);
    };
    b = 10000;
    return innerFunction;
  };

  outerFunction()();

Answer: 10000
```

19. What would be the output of following code?

```
  for (var i = 1; i <= 5; i++) {
    setTimeout(() => {
      console.log(i);
    }, i * 1000);
  }

  Output: 6 6 6 6 6 6
```

20. What would be the output of following code?

```
  for (let i = 1; i <= 5; i++) {
    setTimeout(() => {
      console.log(i);
    }, i * 1000);
  }

  Output: 1 2 3 4 5
```

21. What would be the output of following code?

```
  typeof []

  Output: object
```

22. What would be the output of following code?

```
  typeof (() => {})

  Output: function
```

23. What would be the output of following code?

```
  typeof undefined

  Output: undefined
```
