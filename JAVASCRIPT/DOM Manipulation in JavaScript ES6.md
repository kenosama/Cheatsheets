## Selecting Elements

### document.querySelector()

Selects the first element that matches a CSS selector:
```js
const element = document.querySelector('.my-class');
```

### document.querySelectorAll()

Selects all elements that match a CSS selector:
```js
const elements = document.querySelectorAll('.my-class');
```

## Creating Elements

### document.createElement()

Creates a new element:
```js
const newElement = document.createElement('p'); 
newElement.textContent = 'Hello, World!';
```

## Modifying Elements

### element.innerHTML

Sets or gets the HTML content of an element:

```js
const element = document.querySelector('.my-class'); 
element.innerHTML = '<p>Hello, World!</p>';
```

### element.textContent

Sets or gets the text content of an element:
```js
const element = document.querySelector('.my-class'); 
element.textContent = 'Hello, World!';
```

### element.style

Modifies the inline styles of an element:
```js
const element = document.querySelector('.my-class'); 
element.style.color = 'red';
```

## Adding and Removing Classes

### element.classList.add()

Adds a class to an element:
```js
const element = document.querySelector('.my-class'); 
element.classList.add('new-class');
```

### element.classList.remove()

Removes a class from an element:
```js
const element = document.querySelector('.my-class'); element.classList.remove('my-class');
```

### element.classList.toggle()

Toggles a class on an element:
```js
const element = document.querySelector('.my-class'); element.classList.toggle('new-class');
```

## Adding and Removing Elements

### parentElement.appendChild()

Adds an element as the last child of a parent element:
```js

const parentElement = document.querySelector('.my-parent'); const newElement = document.createElement('p'); parentElement.appendChild(newElement);
```

### parentElement.insertBefore()

Inserts an element before a reference element:
```js
const parentElement = document.querySelector('.my-parent'); const referenceElement = document.querySelector('.my-reference'); const newElement = document.createElement('p'); parentElement.insertBefore(newElement, referenceElement);
```

### parentElement.removeChild()

Removes a child element from a parent element:
```js
const parentElement = document.querySelector('.my-parent'); const childElement = document.querySelector('.my-child'); parentElement.removeChild(childElement);
```


## Listening to Events

### element.addEventListener()

Adds an event listener to an element:
```js

const button = document.querySelector('.my-button'); button.addEventListener('click', (event) => {   console.log('Button was clicked!'); });
```

### element.removeEventListener()

Removes an event listener from an element:
```js

const button = document.querySelector('.my-button'); const handleClick = (event) => {   console.log('Button was clicked!'); }; button.addEventListener('click', handleClick); 

// ...  

button.removeEventListener('click', handleClick);
```

## Getting and Setting Attributes

### element.getAttribute()

Gets the value of an attribute:
```js

const button = document.querySelector('.my-button'); const value = button.getAttribute('data-value');
```

### element.setAttribute()

Sets the value of an attribute:
```js

const button = document.querySelector('.my-button'); button.setAttribute('data-value', '42');
```

## Traversing the DOM

### element.parentNode

Gets the parent node of an element:
```js

const element = document.querySelector('.my-element'); const parent = element.parentNode;
```

### element.childNodes

Gets the child nodes of an element:
```js

const element = document.querySelector('.my-element'); const children = element.childNodes;
```

### element.nextSibling

Gets the next sibling node of an element:
```js
const element = document.querySelector('.my-element'); const nextSibling = element.nextSibling;
```

### element.previousSibling

Gets the previous sibling node of an element:
```js 
const element = document.querySelector('.my-element'); const previousSibling = element.previousSibling;
```
