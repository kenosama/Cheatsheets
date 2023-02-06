## Variables
```js
// let - block scoped
let name = 'John';

// const - block scoped, constant value
const PI = 3.14;
```

## Arrow Functions
```js
// Basic Syntax
const func = (params) => {
  // code
};

// One line syntax, implicit return
const func = (params) => expression;

// No parameters
const func = () => {
  // code
};

// Example
const greet = name => `Hello, ${name}!`;
```

## Template Literals
```js
// Basic Syntax
const name = 'John';
const message = `Hello, ${name}!`;
```

## Destructuring
```js
// Array Destructuring
const numbers = [1, 2, 3];
const [a, b, c] = numbers; //so a=1 b=2 c=3

// Object Destructuring
const person = {
  name: 'John',
  age: 30
};
const { name, age } = person; // so name='john'; & age=30
```

## Classes
```js
// Basic Syntax
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    return `Hello, my name is ${this.name}.`;
  }
}

// Example
const john = new Person('John', 30);
console.log(john.greet()); // Hello, my name is John.
```

## Modules
```js
// Export
export const name = 'John';

// Import
import { name } from './module';
```

## Spread Operators
```js
// Array Spread
const numbers1 = [1, 2, 3];
const numbers2 = [4, 5, 6];
const numbers = [...numbers1, ...numbers2];

// Object Spread
const person1 = { name: 'John' };
const person2 = { age: 30 };
const person = { ...person1, ...person2 };
```

## Axios fetch data from API
```js
import axios from 'axios'; 
const fetchData = async () => { 
	try { 
		const response = await axios.get('https://api.example.com/data'); 
		const data = response.data; 
		return data; 
		}
		catch (error) { 
		throw new Error(error); 
		} 
}; 

const getData = async () => { 
try { 
	const data = await fetchData(); 
	console.log(data); 
	} 
	catch (error) { 
	console.error(error); 
	} 
};
```
