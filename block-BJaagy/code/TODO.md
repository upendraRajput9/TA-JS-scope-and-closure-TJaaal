1. Create a function by your choice that accepts a callback function.

```js
function lastword(arr,opfn){
let newWords=opfn(arr)
return newWords
}

function filterWord(words){
let result = words.filter(word => word.length < 6);
return result
}
lastword([`aray`,`john`,`kilwish`,`carry`,`putipi`],filterWord)
```

2. Create a function by you choice that returns a function reference.
```js
function add(arr,cd){
let output = cd(arr)
return output
}
add([1,2,3,4,5],function(n){
  let value = 0;
  n.map(m=>{
value+=m
  } )
  return value
})
```
3. Create a higher order function called `map` that takes two inputs:
   - An array of numbers/string/boolean etc
   - A 'callback' function - a function that is applied to each element of the array (inside of the function 'map')

Have `map` return a new array filled with values that are the result of the 'callback' function on each element of the input array.

```js
// Your code goes here
function map(arr, opfn) {
  let newArr = []
  arr.map((m) => newArr.push(m*opfn(1)))
  return newArr
}
// Test Your Code
function multiplyByTwo(n) {
  return n * 2
}
map([1, 2, 3, 4, 5], multiplyByTwo) //-> [2,4,6,8,10]
multiplyByTwo(1) //-> 2
multiplyByTwo(2) //-> 4
```

4. Create a higher-order function called `forEach` taht takes an array and a callback, and runs the callback on each element of the array. `forEach` does not return anything.

```js
// Your code goes here
function forEach(arr, opfn) {
  let output = opfn
  output(letters.join(``))
}
// Test Your Code
let alphabet = ''
let letters = ['a', 'b', 'c', 'd']
forEach(letters, function (char) {
  alphabet += char
})
console.log(alphabet) //prints 'abcd'
```

5. Create higher-order function called `filter` takes an array and a callback, and runs the callback on each element of the array if the return value of callback is `truthy` store in new array return the new array.

```js
function filter(arr, opfn) {
  let output = opfn
  let ad = arr.filter((m) => output(m))
  return ad
}
// Test Your Code

var numbers = [1, 3, 5, 4, 7, 89, 234, 20]
let even = filter(numbers, function (n) {
  return n % 2 === 0
})
console.log(even) // [4,234,20]
let odd = filter(numbers, function (n) {
  return n % 2 !== 0
})
console.log(odd) // [1,3,5,7,89]
```
