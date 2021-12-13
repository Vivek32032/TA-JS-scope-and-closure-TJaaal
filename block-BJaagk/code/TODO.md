1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage = function percentage(marks, total){
  return (marks * 100) / total;
}

let percentage = function(marks, total){
  return (marks * 100) / total;
}

let percentage = (marks, total)=>{
  return (marks * 100) / total;
}
let percentage = (marks, total)=>(marks * 100) / total;

```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
//function declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
//function expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// function expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
//function expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;
//function expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
 
 when we assign any function to any variable while declaring it.than it is called function expression 
 ex:- 
 ```js
 let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```

4. Why is a function call an expression in JavaScript?

A function is taken as an expression in javaScript as function in javaScript is an object and we can assign it to any variable.


5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer   Valid 5
five = add; // Answer    valid
five = five(10, 11); // Answer valid 21
five = function () {  
  return 'Hello';
}; // Answer valid
```

6. What is the difference between function definition and function call? Explain with an example.

function definition :- whenever we define a functions with certain stapes it is called function definition and when we call with parenthesis it is called function call
ex:- 
```js
//function declaration
function add(a, b) {
  return a + b;
}
//function call 
add(2,3)
```
7. What is the similarities between function definition and function call?
//function defination is an expression (functions is an object)
//function call is an expression (function call always returns a value)

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid as function hello is an object so we can store key and value pair in it.
```

9. What is higher order function explain with an example.
a function calling or returning function is called higher order function.
//-that accepts a function defination
 //- that return a function defination

10. Explain what is callback function. Why you can pass a function inside a function?

 a function passed as an as an argument in another function is called callback function.