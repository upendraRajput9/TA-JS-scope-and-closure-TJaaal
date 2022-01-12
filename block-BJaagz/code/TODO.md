1. Implement `forEach` array method using Array.reduce

- `forEach` accepts two parameter array and callback
- It does not return anything
- It should work exactly like array `forEach` method

```js
function forEach(arr,opfn) {
arr.reduce((acc,cv,i,a)=>{
return acc = acc.concat(opfn(cv,i,a))
},[])
}

forEach(['Sam', 'Jon', 'Arya'], (name, i, arr) =>
  console.log(name + name, i, arr)
);
```

2. Implement `map` array method using Array.reduce

- `map` accepts two parameter array and callback
- It returns same size of array
- It should work exactly like array `map` method

```js
function map(arr,opfn) {
  // Your code goes here
  let output = opfn
return arr.reduce((acc,cv)=>{
return acc = acc.concat(opfn(cv))
},[])
}


map(['Sam', 'Jon', 'Arya'], (name) => name + name); // ['SamSam', 'JonJon', 'AryaArya']
```

3. Implement `filter` array method using Array.reduce

- `filter` accepts two parameter array and callback
- It returns same size or smaller array
- It should work exactly like array `filter` method

```js
function filter(arr,opfn) {
  // Your code goes here
  
return arr.reduce((acc,cv)=>{
if(opfn(cv)){acc.push(cv)
} 
return acc
},[])

}
filter(['Sam', 'Jon', 'Arya'], (name) =>
  name.startsWith('S')
); // ['Sam']
```
