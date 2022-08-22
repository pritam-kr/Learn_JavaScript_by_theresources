# All about variables

### Real-life example

[https://javascript.info/variables](https://javascript.info/variables)

![Untitled-2022-08-22-1451.excalidraw.png](https://res.cloudinary.com/dhqxln7zi/image/upload/v1661170679/Untitled-2022-08-22-1451.excalidraw_itmgmy.png)

Here, myName is like a box. And myName is the name for that box. 

we can put any value into that box. (can be any value string, boolean, array,  object, number)

In JavaScript, We use variables to store data. 

### Create a variable in JavaScript.

In a Tradition way. we use the **var** keyword to create a variable. You can still see this **var** keyword in old JavaScript code. But we have other ways to declare a variable in JavaScript. using **let** and **const** keywords. Both are new keywords introduced in [ES6 2015.](https://learnersbucket.com/tutorials/es6/var-let-and-const/) 

```jsx
var myName = "Rahul Kumar"

// You can change the value inside a box

myName = "Shubham Kumar"

// But if you enter a new value, the old value gets removed from that variable. 

// You can copy from one variable to another variable

var yourName = myName

console.log(myName, yourName) // Shubham Kumar Shubham Kumar

// Here, both variables are different. 

```

### About var Keyword:-

- You can re-declare with the same variable name.
- You can update the value of a variable.
- It is a function scoped and global scoped.

### Scope:-

The scope is the policy for the visibility of a variable in JavaScript. As I mentioned that var keyword is function and global scoped. 

- **Function Scope** - If a variable declares inside a function, that variable is only accessible inside that function only. You can not access that variable outside of that function.

```jsx
// Function scope

function getName() {
  var myName = 'Shubham Kumar';
}

getName();

console.error(myName); // Error: myName is not defined
```

- **Global Scope -** If your variables declare outside of a function or block scope, which means you can that variable anywhere in the program.

```jsx
// Global Scope

var yourName = 'Rahul Kumar';

function getYourName() {
  console.log(yourName); // Rahul Kumar
}

getYourName();
```

### Rules for variable declaration

- The name must contain a letter, a letter with a digit, or the symbols `$`
 and `_`  But The first character must not be a digit.

```jsx
// Both are two different variables
var myname = "Rahul"

var MYNAME = "Rahul"
```

- when your variable name contains multiple words use [camelCase](https://en.wikipedia.org/wiki/CamelCase) formate.

```jsx
var myHome = "sweet home";

var totalNumber = 56;

var totalProductNumber = 49;
```

### External Links
 
- [All about **var** keyword](https://javascript.info/var)