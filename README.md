### const and let

```javascript
const name = "John";
let age = 24;
```

```javascript
{
  const name = "John";
  let age = 24;
  var country = "Portugal";
}

console.log(name);
console.log(age);
console.log(country);
```

### Arrow functions
```javascript
const sayName = (name = "paulo") => {
  return `<h1>Hello my name is ${name}</h1>`
}

```
### Template strings
```javascript
const name = 'John';
const component = `<h1>Hello my name is ${name}</h1>`;
```
### Default params
```javascript
const sayName = (name = "paulo") => {
  return `<h1>Hello my name is ${name}</h1>`
}

console.log(sayName());
console.log(sayName('John'));

```
### Rest
```javascript
const names = (a, b, ...manyMoreArgs) => {
  console.log(a, b, manyMoreArgs); 
}

names("john", "cindy", "paul", "mike", "guru");

```
### Spread

```javascript
const firstRow = [1,2,3,4];
const secondRow = [5,6,7,8];

console.log([...firstRow, ...secondRow]);
console.log([...firstRow, ...secondRow, 9, 10]);

const firstRowCopy = [...firstRow];

[...document.querySelectorAll('div')];
```
###  Destructuring
```javascript
const data = {
  name: "John",
  age: 25,
  country: "Portugal",
}

console.log(`Hello my name is ${data.name}, im ${data.age} years old and i'm from ${data.country}`);

const {name, age, country} = data;

console.log(`Hello my name is ${name}, im ${age} years old and i'm from ${country}`);

```
### Foreach
```javascript
let data = [{
  name: "John",
  age: 25,
  country: "Portugal",
}]

data.forEach(item => {
  item.name = 'Mike';
})

console.log(data);

```
### Map
```javascript
let data = [{
  name: "John",
  age: 25,
  country: "Portugal",
}]

data.map(item => {
  item.name = 'Mike';
})

console.log(data);
```

### Filter
```javascript
const data = [2, 3, 4, 2, 5, 2, 6, 2, 7];

const newData = data.filter(item => item !== 2);

console.log(newData);
```

### Find

```javascript
const data = [2, 3, 4, 2, 5, 2, 6, 2, 7];

const newData = data.find(item => item > 5);

console.log(newData);
```

###  Every 
```javascript
const data = [2, 3, 4, 2, 5, 2, 6, 2, 7];

const newData = data.every(item => item > 5);
const newData2 = data.every(item => item > 1);

console.log(newData);
console.log(newData2);

```

### Some
```javascript
const data = [2, 3, 4, 2, 5, 2, 6, 2, 7];

const newData = data.some(item => item > 5);
const newData2 = data.some(item => item > 10);

console.log(newData);
console.log(newData2);

```

### Reduce
```javascript
const data = ["batman", "aquaman", "wonder woman"];

const newData = data.reduce((prev, next) => {
  return `${prev} vs ${next} \n`;
})

console.log(newData);

const data = [1, 2, 3];

const newData = data.reduce((prev, next) => {
  return prev + next;
})

console.log(newData);

```

## Ternary
```javascript
const isTrue = true;

isTrue ? 'It works' : 'No way';

```

## Classes
```javascript
class Cat {
  constructor(name = 'no name', color ='no color', age = "no age" ){
    this.name = name;
    this.color = color;
    this.age = age;
  }
  
  sayName(){
    return `My name is ${this.name}`;
  }
  
  sayColor(){
    return `My name is ${this.color}`;
  }
  
  sayAge(){
    return `My name is ${this.age}`;
  }
}

const zebra = new Cat();
const kitty = new Cat('Kitty', 'orange', 5);


```
