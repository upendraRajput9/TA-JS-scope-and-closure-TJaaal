1. What does thread of execution means in JavaScript?
Answer:Thread execution mean when we want to execute code. JavaScript engine take this code execute line by line.
2. Where the JavaScript code gets executed?
Answer: The JavaScript code gets executed in global excution context.
3. What does context means in Global Execution Context?
Answer: The Environment Where code get executed.
4. When do you create a global execution context.
Answer: Globle execution context is the first execution context that get created by JS engine whenever it is running your code for the first time and that created only one when JS engine running your code.

5. Execution context consists of what all things?
Answer:Execution context consists of variable scope, function arguments, and the value of the this object
6. What are the different types of execution context?
Answer:There are two type of execution context are:-
1- Global execution context;One get created only once throughtout the program.
2- And other one known as functiion execution context that gets created whenever we are executing any code.

7. When global and function execution context gets created?
Answer:1- Global execution context;One get created only once throughtout the program.
2-  Functiion execution context that gets created whenever we are executing any code.
8. Function execution gets created during function execution or while declaring a function.
Answer:Function execution gets created during function execution

9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./WhatsApp Image 2022-01-06 at 16.58.31 (1).jpeg)




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

![](./WhatsApp Image 2022-01-06 at 16.58.31 (2).jpeg)



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

![](./WhatsApp Image 2022-01-06 at 16.58.31.jpeg)