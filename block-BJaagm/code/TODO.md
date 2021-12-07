1. What does thread of execution means in JavaScript?

javascript engine executes the code line by line this is called thread of execution.

2. Where the JavaScript code gets executed?
javascript code gets executed in global execution context.

3. What does context means in Global Execution Context?
This is the 'environment' a function executes in which JS code start its execution when the file first loads in the browser.

4. When do you create a global execution context.
   JavaScript engine creates the global execution context before it starts to execute any code.

5. Execution context consists of what all things?

6. What are the different types of execution context?
two type of execution context :- global execution context and function execution context

7. When global and function execution context gets created?
global execution context gets created by javascript engine before executing any piece of code.
and function execution context created after calling function

8. Function execution gets created during function execution or while declaring a function.
//during function execution.

9.  Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)