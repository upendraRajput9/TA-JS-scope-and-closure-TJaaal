Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); // `username is not defined`
```
In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the object named `Arya` and we can't access the variable defined inside a object from outside.

The above code will throw an error `ReferenceError: useranme is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // `useranme is not defined`
```
In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the if statement named `Arya` and if needs a expression if expression is 
true then access the variable defined inside a object from outside.
The above code will throw an error `ReferenceError: useranme is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // useranme is not defined
```
In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the if statement named `Arya` and if needs a expression if expression is 
true then access the variable defined inside a object from outside.
The above code will throw an error `ReferenceError: useranme is not defined`.


5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // `'username' has already been declared`
```
In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope. And another same  variable is inside the if statement named `Arya` is defined by using var scope
so that the above code will throw an error `SyntaxError: Identifier 'username' has already been declared`.


6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // John
```
In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope. And another same  variable is inside the if statement named `Arya` is defined by using let scope
so we cannot access the a varible that is not initialized.
 


7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // John
```
In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope. And another same  variable is inside the function named `Arya` is defined by using let scope
so we cannot access the variable outside the function.

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 'First', 1 'First',2 'First', 3 'First', 4 'First',5 'First',6 'First',7 'First',8'First',9 'First'
}
console.log(i, 'Second'); //  10 'Second'
```
In above code we are looking for the variable named `usename`.There is a variable named `username` in the for loop is define by using var scope so it is initialized and it access out side in global scope.

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); //  0 'First', 1 'First',2 'First', 3 'First', 4 'First',5 'First',6 'First',7 'First',8'First',9 'First'
}
console.log(i, 'Second'); // i is not defined
```
In above code we are looking for the variable named `usename`.There is a variable named `username` in the for loop is define by using let scope so it is not initialized and it is not access out side in global scope.

so that the above code will throw an error `ReferenceError: i is not defined`.