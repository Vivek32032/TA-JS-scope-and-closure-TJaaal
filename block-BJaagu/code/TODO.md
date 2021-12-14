Find the output of the code snippets below:

```js
console.log(numA + numB); //OUTPUT NaN
var numA = 21,
  numB = 30;
```
here namA and numB is equal to  undefined in global exection context so if we add undefined with undefined we have NaN as an output.
Find the output of the code snippets below:

```js
console.log(numA + numB); //OUTPUT  numA is not defined
let numA = 21,
  numB = 30;
```
since variable numA is defined with let keyword therefor it will not have any value in global declaration context
hance it will throw an error as numA is not defined before console-log method.

Find the output of the code snippets below:

```js
let numA = 21,
  numB = 30;
console.log(numA + numB); //OUTPUT 51
```
since variable numA is defined with let keyword therefor it will not have any value in global declaration context
but since console.log is after declaration of namA and numB
hance it will console the value of sum of namA and numB.

```js
console.log(sayHello()); // OUTPUT  "Hello"
function sayHello() {
  console.log("Hey");
}
function sayHello() {
  console.log("Hello");
}
``` 
here function sayHello is declared again so it will replace first declaration. and when called second declaration of steps will execute

Find the output of the code snippets below:

```js
let username = "Tyrion";
sayHello(); // OUTPUT   "Tyrion"
function sayHello() {
  console.log(username);
}
```
here, `username` is declared in global scope so when we call sayHello function it will get the value of `username` as "Tyrion" and so output will be "Tyrion";

Find the output of the code snippets below:

```js
sayHello(); // OUTPUT ReferenceError: username is not defined  at sayHello
let username = "Tyrion";
function sayHello() {
  console.log(username);
}
```
here, we are calling the sayHello function before declaring username therefore it will throw an reference error.


Find the output of the code snippets below:

```js
let username = "Tyrion";
sayHello(); // OUTPUT  ReferenceError sayHello is not defined
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

```js
sayHello(); // OUTPUT  ReferenceError sayHello is not defined
let username = "Tyrion";
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

```js
sayHello(); // OUTPUT  ReferenceError sayHello is not defined
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
sayHello(); // OUTPUT ReferenceError sayHello is not defined
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  var username = "John";
};
sayHello(); // OUTPUT undefined
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  var username = "John";
  console.log(username);
};
sayHello(); // OUTPUT "John" 
```
when sayHello is called it will first search the variable in local scope and it will find `username` value as "John" so it will console-log "John".

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  let username = "John";
};
sayHello(); // OUTPUT 'username' before initialization at sayHello