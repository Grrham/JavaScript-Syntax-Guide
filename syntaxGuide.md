
#                   **Welcome**
##             Java Script syntaxGuide
###                  By:[Benton]

###               **Variables**

Variables can be declared using 3 keywords:
- `const`
- `let`
- `var`

**const**

Use const when the value or type shouldn't be changed, const cannot be reassigned  after its initial value is assigned.

```javascript
const a = 1;
const b = 2;
const c = a + b;
```

**let**

Use let for variables that will need to be reassigned.

```javascript
let message = "Hello World!";
```

**var**

Should only be used when writing code for older browsers - pre 2015.

```javascript
var name = "John";
var age = 30;
```

**Variable Naming**

- Variable names must begin with a letter, dollarsign or underscore
- They are case-sensitive
- Use propper wording to improve coding readability

**Assign // Reassign**

Use '=' to assign a value to a variable.

```javascript
let x = 10;
```

- you can simply reasign x by stating:

```javascript
x = 10;
```

- however this only works when declared with `let`.
`const` variables can __NOT__ be reassigned

### **Comaprison Statements**

Comparison statements are used to compare values in JavaScript. 

+ Common comparison operators include:
- `== equal`
- `!= not equal`
- `< less than`
- `> greater than`
- `>= greater than or equal to`
- `<= less than or equal to`

**Equal (==) and Not Equal (!=)**

```javascript
let firstNumber = 5;
let secondNumber = 3;

if (firstNumber == secondNumber) {
  console.log(`The first number is equal to the second number.`);
} else {
  console.log(`The first number is not equal to the second number.`);
}

if (firstNumber != secondNumber) {
  console.log(`The first number is not equal to the second number.`);
} else {
  console.log(`The first number is equal to the second number.`);
}
```

**Greater Than (>) and Less Than (<)**

```javascript
let age = 20;
let legalAge = 18;

if (age > legalAge) {
  console.log(`This person is older than the legal age.`);
} else {
  console.log(`This person is not older than the legal age.`);
}

if (age < legalAge) {
  console.log(`This person is younger than the legal age.`);
} else {
  console.log(`This person is not younger than the legal age.`);
}
```

**Greater Than or Equal To (>=) and Less Than or Equal To (<=)**

```javascript
let speedLimit = 60;
let currentSpeed = 70;

if (currentSpeed >= speedLimit) {
  console.log(`The vehicle is either at or above the speed limit.`);
} else {
  console.log(`The vehicle is below the speed limit.`);
}

if (currentSpeed <= speedLimit) {
  console.log(`The vehicle is at or below the speed limit.`);
} else {
  console.log(`The vehicle is above the speed limit.`);
}
```

### **Boolean Statements**

Boolean statements involve logical conditions in JavaScript. They are often used in control structures like `if` statements and loops.

**True and False**

You have two boolean values: `true` and `false`.

```javascript
let isTrue = true;
let isFalse = false;
```

**Logical Operators**

These are used to determine logic between values or variables.

+ The operators include:
- `&&` (and)
- `||` (or)
- `!` (not)

```javascript
let x = 5;
let y = 4;

(x < 10 && y > 1) is true
// this example states that 10 is larger then x and y is greater than 1


(x == 3 || y == 3) is false
// x is equal to 3 OR y is equal to 5


!(x == y) is true
// the ! says that x is not equal to y
```

### **Arrays**

Arrays are used to store multiple values in a single variable.

**Declaration and Initialization**

You can create arrays by stating:

```javascript
let fruits = ["apples", "oranges", "bananas"];
```

- To access a value within that string you must use square brackets and a index to target it, for example:

```javascript
let firstFruit = fruits[0]; // this will target the first value
```

- Index starts at 0 so if you want the first value in a array you must use 0

**Modifying Arrays**

To modify, add, or delete a element you can use:

```javascript
fruits.push("mangos"); // .push will add "mangos" to the end if the array
fruits.pop(); // .pop removes the last element in the array
fruits[1] = "grapes"; // this will replace the second element in the array with "grapes"
```

### **Objects**

Objects are like variables but can contain many values.

**Object Declaration**

You can create objects in JavaScript like this:

```javascript
let user = {
  name: "John",
  age: 30,
};
```

**Accessing Object Properties**

```javascript
user.name; // this accesses "John"
user["age"] // this accesses "30"
```

- using `.property` or `["property"]` are both valid ways to target

**Modifying Objects**

```javascript
user.city = "New York"; // adds a new property under the object
user.age = 20; // changes the age to 20
delete user.age; // deletes the age property
```

### **Functions**

A function is a block of code designed to exicute a particular task.

**Function Declaration**

Functions are defined by using the `function` keyword followed by a name.

```javascript
function sayHi(){
  console.log("Hello, World!");
}
// then you can call the funstion by stating:
sayHi();
```

- functions can also return values

```javascript
function add(a, b){
  return a + b;
} // in this case a and b are placeholders so i can replace them with say 5 and 4:
add(5, 4) // and the console will add the 2 numbers together giving me 9
```

### **Functions & Parameters**

Functions can also accept parameters.

```javascript
function greet(name){
console.log("Hello, " + name + "!");
} // i can now call this function by saying 
greet("Benton"); 
```

- Doing so will replace `name` with `Benton` and give me:

```javascript
Hello, Benton!
```

### **Loops**

Loops can allow you to execute a block of code repeatedly.

**`for` Loop**

Used to execute a block of code a specific number of times.

```javascript
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

- This loop counts from 1 to 5 and logs each number to the console

**`while` Loop**

Executes a block of code while a specific conidtion is true.

```javascript
let i = 1;
while (i <= 5) {
  console.log(i);
  i++;
}
```

- This loop is simular to the `for` loop howover uses `while` which is exicuting the code aslong as 1 is less then or equal to 5

### **Data Types**

JavaScript supports various data types, including numbers, strings, booleans, bigint, objects, symbols, arrays, null and undefined.

**Numbers**

- For numbers of any kind

```javascript
let num = 22;
```

**Strings**

- A series of characters like: `John Doe`

```javascript
let text = "John, Doe";
```

**Booleans**

- Has 2 values `true` or `false`

```javascript
let isTrue = true;
let isFalse = false;
```

**BigInt**

- Simular to `numbers` but used to represent intergers of abitrary length

```javascript
let bigNum = 2038495427487957292;
```

**Objects**

- Used to store collections of data

```javascript
let user = {name: "John" , age: 22};
```

**Symbols**

- Typically used as a `object` property for unique identifiers

```javascript
let sym = Symbol("description");
```

**Arrays**

- Used to store multiple values in a variable

```javascript
let numbers = [1, 2, 3, 4, 5];
```

**Null & Undefined**

- Null is the intentional absense of a object value
- Undefined is used for variables that dont yet have a value

```javascript
let data = null;
let value;
console.log(value);
```

- In this case the console will output `undefined` because the `variable` doesnt have any `value` that exists yet

### **Comments**

Comments are used for explaing and adding notes into your code.

**Single-Line Comments**

- Use `//` for single-lines

```javascript
// this is a single line comment
```

**Multi-Line Comments**

- Use `/*___________*/` for multi-lines

```javascript
/*
this is a multi-line comment in javaScript,
tt can span multiple lines and is useful for providing
detailed explanations or commenting out large sections
of code 
*/
```