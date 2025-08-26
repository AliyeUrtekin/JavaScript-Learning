# VARIABLES
### What is a variable?
A variable is a container for a value. (Variables are containers for storing values.)

## Declaring a Variable
Creating a variable in JavaScript is called "declaring" a variable.

JavaScript variables can be declared in 4 ways:

- Automatically
- Using **var**
- Using **let**
- Using **const**

### Automatically
**Example:** In this first example x, y, and z are undeclared variables. They are automatically declared when first used:

```js
x = 3;
y = 4;
z = x + y;
```
From the examples you can guess:

- x stores the value 3
- y stores the value 4
- z stores the value 7

### var 
The **var** keyword was used in all JavaScript code from 1995 to 2015.

The *let* and *const* keywords were added to JavaScript in 2015.

The var keyword should only be used in code written for older browsers.

*Function-scoped* (limited to the function where it is declared).

Can be redeclared and updated.

Hoisted -> JavaScript moves it to the top of its scope but initilizes it with `undefined`.

### let
Introduced in ES6 (2015).

*Block-scoped* (limited to `{ }` where it's declared).

Can be updated (re-assign) but not redeclared in the same scope.

```js
let age = 29;
age = 30; //update allowed
console.log(age) //30
```
### const
Also introduced in ES6.

*Block-scoped* like `let`.

Must be initialized when declared.

Cannot be reassigned (constant).

Good for values that shouldn't change.

```js
const birthYear = 1991;
console.log(birthYear); //1991

//birthYear = 2001; X Error: Assignment to constant variable
```

**Note:**`const` does **not make objects immutable**. You can still change properties inside an object/array:

```js
const person = { name: "Nico" };
person.name = "Velti"; // allowed
console.log(person); // { name: "Velti" }
```

## Initializing a Variable
Initializing a variable means assigning an initial value to a variable at the time it is declared or later, so it holds something instead of being `undefined`.

```js
// Declaration without initialization - When you just declare a variable without assigning a value, it will automatically hold the value undefined.
let age; // declared but not initialized
console.log(age); // undefined

//Declaraiton with initialization - When you both declare and assign a value in one step.
let age = 27; // declared + initialized
console.log(age); // 27

// Later initialization - You can also declare first, then initialize later:
let name;  // declaration
name = "John"; // initialization
console.log(name); // John
```

**Initialization** is the process of giving a variable its first value.




