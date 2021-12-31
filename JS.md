# Javascript CheatSheet

## Main brackets

- `{ }`: is mainly used for Scopes, where we define the `function` body, `if` statement body, `switch` body, `else` body, and all the other syntaxes that need a scope.
- Also it can be used for objects {key: value}

- `( )`: is mainly used for functions parametrs, and conditional statments conditions
- `[ ]`: is mainly used for arrays, and dynamically accessing objects.

## Javascript Basics

**Comments**

Comments in javascript are in the following format

```js
/* This 
is
a 
multiline
comment */

// this is a single line comment
```

**Variables and constants**

`let`: for variables
`const`: for constants

```js
// to create a new variable
let x = 4;
// to create a new constant
let pi = 3.14;
```

**Main Types:**

```js
// Number:
let a = 5;
let a = 5.73341;
// String:
let b = "Hello";
let b = "Hello";
let b = `Hello`;
// Boolean:
let c = true;
let c = false;
let c = 5 == 5;
let c = 5 > 5;
```

**Print**
To print out on the console

```js
// 1. printing string
console.log("Hello World"); // -> Hello World

// 2. printing values inside stored variables or constant
const pi = 3.14;
console.log(pi); // 3.14

// 3. printing more than one element,
const x = 5;
const y = 10;
console.log(x, "Hello World", y); // 5 Hello World 10

// 4. console.log adds one line after it finishes
console.log(); // will just print an empty new line
```

### Basics

#### Strings

Anything in javascript between `" "` or `' '` or back ticks ` `` ` is called a string
Every text should be between quotation marks.

**Special Characters**

```js
console.log("\n"); // prints a new line
console.log("\t"); // prints a tab   space
console.log('"'); // prints a single back slash \
console.log('"'); // prints a single back slash \
console.log("________"); // prints a single quotation mark "
```

**String Interpolation**
To add values inside a string we use the back tics `` `TEXT ${VARIABLE or COMPUTATION} TEXT` ``

```js
const x = 1;
const y = 100;
console.log(`x: ${x}, y: ${y}`); // prints: x:1, y:100
console.log(`x: ${x}, y: ${y}`); // prints: x:1, y:100
console.log(`${x + y}`); // prints: 101
```

**Mathmatical operations**

```js
// addition
10 + 5;

// subtraction
10 - 5;

// multiplication
10 * 5;

// division
10 / 5;

// remainder: The reminder of the division
10 % 5;
```

#### If statement

**Logical operations**

```js
// Equals
"5" == 5; // returns true

// Strictly Equals (Better usage: returns true if same value, same type)
"5" === 5; // returns false

// doesn't equal
5 != 5; // returns false

// strictly doesn't equal
5 !== 5; // returns false

// greater than
10 > 5; // returns true

// greater than or equal
10 >= 10; // returns true

// less than
10 < 5; // returns false

// less than or equal
10 <= 5; // returns false

// connects 2 booleans, both of them should be true to make the final result true
10 > 5 && "Hello" == "Hi"; // returns false, because the second one is false

// connects 2 booleans, one of them should be true to make the final result true
10 > 5 || "Hello" == "Hi"; // returns true, because the first one is true
```

**If Statement**

```js
// The condition inside the () should return either true or false
const x = 5;
if(x === 5){
  // statement that will be executed if the condition was true
}

// You can link the if statement with else to execute if the condition was false

const x = 5;
if(x!=5){
  // do job 1
}
else{
  // do job 2
  // This code will only be execute if only the condition inside the if didn't work
  // you don't put a condition after the else statement
}

// The if chain, only one of the following jobs will be executed
if(CONDITION){
  // job 1
}
else if(CONDITION 2){
  // job 2
}
else of(CONDITION 3){
  // job 3
}
else{
  // job 4
}
```

There are some rules for the if chain

1. You can only have `else if`s between if and else
2. You cannot add `else` after `else`
3. One job only the if chain will be executed, even if the other `else if`s conditions where true

**Reminder %**
We use the reminder `%` for couple of usages, most importantly, knowing even or odd numbers.
Even numbers will return true on the following statement

```js
const x = ???
// if you want to check if x is even, you do the following condition
if(x % 2 == 0){
  // will only be executed if x was event
}
```

---

# Functions

You deal with functions in 2 main things

1. Function creation
2. Function execution (invoking)

```js
// 1. function creation
function foo() {
  // This code will be executed when you call (invoke) the function
}

// 2. To invoke (call) the function
foo();
```

**parameters and arguments**

- We call them parameters from the outside when we call the function
- We call them arguments from the inside when we create the function

```js
// 1. Function that takes multiple arguments
function foo(arg1, arg2, arg3) {}

// 2. Calling the function and passing multiple parameters
foo(1, 2, 3);
```

**Return**
A function can return using the command `return` by the end of the function

```js
// this function for example returns the square of any number you plug it
function square(x) {
  return x * x;
}
console.log(square(4)); // this will log 16
```

> **COMMON MISTAKE**
> When we return, we use the console.log to log the returned value. Lots of times, we do the mistake of trying to console.log inside the function.

```js
function pi() {
  return 22 / 7;
}
console.log(pi()); // console.log outside not inside
```

---

# Arrays

You can put groups of elements

```js
// New array
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 90];
```

**Accessing elements**

```js
const array = [100, 90, 80, 40];

// To access the first element
array[0];

// To access the second element
array[1];
//
```

**Length**

```js
const array = [100, 90, 80, 40];

array.length; // returns number of elements in the array
console.log(array.length); // prints number of elements in the array
//
```

**Length usages: Getting the last element in the array**

```js
const array = [100, 90, 80, 40];

// to get the last element in the array
array[array.length - 1];
```

**push and pop**

```js
array.push(NEW_ELEMENT); // adds a new element
array.pop(); // removes the last element
//
```

# Loops

There are 2 main loops

1. `for` loop
2. `while` loop

```js
while (condition) {
  // keeps looping while the condition is true
}

for (let i = 0; i < 10; i++) {
  // initializes a counter
  // keeps looping while the condition is true
  // and increments on every loop
}
```

# Iteration Methods And Arrow Functions

### Arrow functions

```js
// the function way
function foo() {}
// the arrow function way
const foo = () => {};
```

### Iteration Methods

- Iteration methods work on **ARRAYS** only!
- All iteration methods go over every single element of the array
- Iteration methods take a function that has a parameter of the current value of the array. Preferred to use arrow function inside it.

```js
array.SOME_ARROW_FUNCTION((element) => {
  // Whatever action you want to perform on every single element
  // Most arrow functions will require you to return something
  // The only arrow function that doesn't require to return something is `forEach`
});
```

The following are the main iteration methods

1. `.forEach`: just goes over all the elements, doesn't return anything, and doesn't require you to pass a function that returns anything
2. `.filter`: returns a filtered copy of the array that is based on a condition that you return from the function you pass it.
3. `.map`: returns a transformed copy of the array that is based on a returned shape of every element that you return from the function you pass it
4. `.find`: looks exactly like `.filter`, but it only returns the first element that matches the condition
5. `.some`: looks exactly like `.find`, but it only returns true if it finds 1 element that matches the condition
6. `.reduce`: returns a single value that is compiled through the whole array using `previous` and `current` values being passed in passed function. We usually use it to get the sum

```js
const array = [10, 20, 30, 40, 50, 60];
array.map((e) => e / 10); // returns a transformed array equals to [1,2,3,4,5]
array.filter((e) => e <= 30); // returns a filtered array equals to [10, 20, 30]
array.find((e) => e === 20); // returns 20
array.some((e) => e === 20); // returns true
array.reduce((prev, current) => prev + current); // returns the sum of the array (210)
```

# Objects

The structure of object is a pair of `key:value`

```js
// To create an object
const object = {
  PROPERTY_NAME: VALUE,
  "PROPERTY NAME 2": VALUE, // if there are spaces, you can use the quotation marks
};

// to access one element of the object, we have couple of ways
object.PROPERTY_NAME;
object["PROPERTY_NAME"]; // we use this for dynamic access
```

## Accessing the object dynamically

```js
const someObj = {
  key1: "value1",
  key2: "value2",
};
const keyName = "value1";
console.log(someObj[keyName]);
```

## Adding new properties to the object

```js
const someObj = {
  key1: "value1",
  key2: "value2",
};
someObject.key3 = "value3";

/* the object will look like
someObj = {
  key1: "value1",
  key2: "value2",
  key3: "value3"
};
*/
```

# Classes

Classes only have 2 main things to write inside them

1. **Methods**: They are just functions inside a class
2. **Properties**: They are just variables or constants
   You can't execute a function inside the class body, it should only be inside methods.

```js
// to create a new class
class ClassName {}

// creating object
const object = new ClassName();

// Adding properties to the class (without a constructor)
class ClassName {
  name = "Ali";
  age = 3;
}
```

### Creating Methods

```js
class ClassName {
  // the ordinary function way
  foo() {}

  // the arrow function way
  foo = () => {};
}
```

### Constructor

A constructor is just a special **method** that has the following features

1. It gets executed when you create an object from the class using the `new` keyword
2. It's used to initialize the properties
3. It has no name

```js
// creating the constructor
class ClassName {
  // Adding a proeprty that doesn't exist in the constructor
  height = 0;
  constructor(name, age, interests) {
    this.name = name;
    this.age = age;
    this.interests = interests;
  }
  addPropery(propertName, propValue) {
    this[propertyName] = propValue;
  }
}
```

### Inheritance

```js
class ParentClassName {}
class ChildClassName extends ParentClassName {}
```
