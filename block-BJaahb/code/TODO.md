Create the execution context diagram for the following code snippets:

```js
function outer() {
  let b = 10;
  function inner() {
    let a = 20;
    console.log(a + b);
  }
  return inner;
}
let getSum = outer();
let num = getSum();
```
![img1](img/img1BlockBJaahb.png)

2.

Create the execution context diagram for following code. Also write the output of the code below.

```js
function getCounter() {
  let count = 0;

  return () => {
    return count++;
  };
}

let counter = getCounter();

counter(); // output   0
counter(); // output   1
counter(); // output   2
counter(); // output   3
```
![img2](img/img2BlockBJaahb.png)

3. Create the execution context diagram

```js
function makeColorChanger(color) {
  return function () {
    document.body.style.backgroundColor = color;
  };
}

let blue = makeColorChanger('blue');
let tomato = makeColorChanger('tomato');

blue();
tomato();

// What will be the background color after the execution of last line

//tomato
```
![img3](img/img3BlockBJaahb.png)
