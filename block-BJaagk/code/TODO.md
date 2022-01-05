1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage = function (marks, total) {
  return (marks * 100) / total;
}

let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
}


let percentage = function (marks, total)=> {
  return (marks * 100) / total;
}

let percentage = (marks, total) =>
  (marks * 100) / total;

```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
//Function Declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
  //Function Expression
};
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
  //Function Expression
};
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
  //Function Expression
};
```

```js
let percentage = (marks, total) => (marks * 100) / total;
//Function Expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
function definition an expression in JavaScript because it allow us to create anonymous function which doesn't have any function name.
Ex; 
```js
let addnumber = function (numA,numB){
  return numA+numB;
}
  ```

4. Why is a function call an expression in JavaScript?
used to execute a specified function with the provided arguments.
5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer valid because it stored in varible 
five = add; // Answer valid because function store in the varible
five = five(10, 11); // Answer valid because it stored in varible 
five = function () {
  return 'Hello';
}; // Answer  valid because it a fuction expression 
```

6. What is the difference between function definition and function call? Explain with an example.
The difference between function definition and function call is A function is procedure to achieve a particular result while function call is using this function to achive that task
ex: 
```js
function add(numA,numB){
return numA + numB
}

add(34,345);
```
7. What is the similarities between function definition and function call?
it both use to achive result
8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid 
```

9. What is higher order function explain with an example.
Higher order function is a function that accept a function as a perameter or return function.
ex:- 
```js
const numbers = [1, 2, 3, 4, 5];

numbers.forEach((number) => console.log(number + 1));
```
10. Explain what is callback function. Why you can pass a function inside a function?
Any function that is passed as an argument to another function so that it can be executed in that other function is called as a callback function. 


