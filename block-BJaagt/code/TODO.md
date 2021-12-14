Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // output reference Error username is not defined
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and it is created using var keyword and var is function scoped so we can't directly access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

1. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // username is not defined
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside a block and since it is defined using const we can't access it from outside the block as const is block scoped.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.bl

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // username is not defined
```
`username` is defined under the block of if condition so we can't access from outside as it is created using let keyword and let is block scoped.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya'; 
}
console.log(username); // output
```
`username` is defined under the block of if condition even if we can access it from outside as it is created using var keyword and var is not block scoped.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // output
```
here `username` is created using let keyword and again inside if statement we are going to create new variable using var of same name and var is not block scope so it will through an error as we are trying to create same variable again in global scope.

`error` username is already created 
 

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // output 'John'

```
here `username` is created using let keyword and inside if statement again username variable is created with let keyword but it is within the roscope of if statement so it will not throw any error and since we are access the username form outside "John" will get displayed  in our console. 

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // output 'John'
```
here `username` is created using let keyword and again inside function sayHello we are creating `username` with let keyword so it will not throw any error as let create variable of block scope hence this variable will be access with function sayHello and we are consol-logging `username` from outside function `sayHello` hence 'John' will console-log in this case.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First');
}
 // output  
// 0 'First'
// 1 'First'
// 2 'First'
// 3 'First'
// 4 'First'
// 5 'First'
// 6 'First'
// 7 'First'
// 8 'First'
// 9 'First'
console.log(i, 'Second'); // output  10 'Second'
```
here `i` is created using var and var is not block scoped so we can access the value of  `i` globally. 

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
 // output  
// 0 'First'
// 1 'First'
// 2 'First'
// 3 'First'
// 4 'First'
// 5 'First'
// 6 'First'
// 7 'First'
// 8 'First'
// 9 'First'
console.log(i, 'Second'); // output i is not defined
```
since `i` is defined using let keyword inside the block of for loop we can't access `i` keyword from outside so it will throw an error if we are trying to access it from outside the for loop.