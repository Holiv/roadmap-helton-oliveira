# The Complete JavaScript Course

Address: https://www.udemy.com/course-dashboard-redirect/?course_id=851712
Start Date: July 25, 2022
Status: In Progress
Type: Course, JavaScript


* <a href="#values">Values and Variables </a>
    * Convention and Rules to name Variables
* <a href="#data"> Data Types</a>
    * Number
    * String
    * Boolean
    * Undefined
    * Null
    * Symbol (ES2015)
    * BigInt
* <a href="#let"> Let, Const and Var</a>
    * Let
    * Const
    * Var
* <a href="#basic"> Basic Operators</a>
* <a href="#operator"> Operator precedence</a>
* <a href="#stringAndTemplate"> String and Template literals</a>
* <a href="#ifElse"> If/Else statements</a>
* <a href="#typeConversion"> Type Conversion and Coercion</a>
    * Type conversion
    * Type coercion
* <a href="#truthy"> Truthy and Falsy values</a>
* <a href="#equality"> Equality operators</a>
    * loose equality operator (==)
    * strict equality operator (===)
    * Different operator (!= / !==)
* <a href="#boolean"> Boolean Logic (true or false)</a>
* <a href="#logical"> Logical Operators (&&, ||, !)</a>
* <a href="#switch"> The Switch statement</a>
* <a href="#statements"> Statements and Expressions</a>
    * Expression
    * Statement
* <a href="#conditional"> The Conditional (Ternary) Operator</a>
* <a href="#activate"> Activate Strict Mode</a>
* <a href="#functions"> Functions</a>
    * Returning a value from a function
* <a href="#declaration"> Function Declarations vs. Expressions</a>
    * Function Declaration
    * Expressions (Anonymous Function)
    * Real difference between Function Declarations and Function Expressions
* <a href="#arrow"> Arrow Functions</a>
* <a href="#calling"> Functions Calling other Functions</a>
* <a href="#reviewing"> Reviewing Functions</a>
    * Types of function that can be used</a>
    * Anathomy of a function
* <a href="#arrays"> Introduction to Arrays</a>
* <a href="#basicArray"> Basic Array Operations(Methods)</a>
    * Push
    * Unshift
    * Pop
    * Shift
    * IndexOf
    * Includes
* <a href="#objects"> Introduction to Objects</a>
* <a href="#dot"> Dot vs Bracket Notation</a>

# A Brief Introduction to JavaScript

JavaScript is a high level, multi-paradigm, object-oriented programming language.

As a high level language JavaScript doesn’t work with complex stuff like memory management, it makes JavaScript a lot easier to learn and write.

JavaScript is algo based on objects for storing most kind of data and is a Multi-Paragim language that means we can use different styles of programming, as imperative and declarative style.

## <a id='values'> Values and Variables</a>

Value is basically a piece of data. The smallest unit of information in a program. 

It would be extremely useful to reuse values and for the we use variables.

A variable is a box where we can store things (values) and recover these things always we wanted to use them.

```jsx
//showing a value - this value will only be used once.
console.log('Helton');
//storing the same value in a variable, this way the value could be used again.
let firstName = "Helton";
console.log(firstName);
```

### Convention and Rules to name Variables

The most used is the Camel Case convention, it means when we have a variable with two of more names together the second name will start uppercased.

In the past code we have used the variable named **firstName**, as we can see the first word started lowercased and the second uppercased. All the subsequence words will going to start uppercased.

- Variables can never start using numbers
- Variables only can be named using letters, numbers (not starting with), underscores and dollar sign.
- Variables also can’t be named using **keywords** from JavaScript, ***function, new, class,***  and others.
- Variables that start with uppercase character are variables related to Object-Oriented.
- Variables that are written completely in uppercase are variables reserved to Constants. These are variables whose value won’t change.
- Make sure the variables names are very descriptive, it means that the name of the variable is completely correlated with its value. For example ***fistName*** lead us to understand at first sight the it holds a value that is someone first name.

## <a id="data">Data Types</a>

Each value in JavaScript is a **object** or a **primitive value**

```jsx
//JavaScript Object
let me = {
	name: 'Helton'
}
//JavaScript Primitive Value
let firstName = 'Helton';
let age = '30';
```

Value is only primitive value when it is not an object.

***There’s sevem types of primitive values:***

### Number

Floating numbers, used for decimal and integers.

```jsx
let age = '30';
```

### String

Sequence of characters used for text.

```jsx
let name = 'Helton';
```

*Helton* is a sequence of six characters that we call as **string**

Always used with quotes (simples quotes or doble quotes).

### Boolean

Logical type that can only be **true** or **false**, used for taking decisions.

```jsx
let fullAge = true;
```

These three types above are the main types used in JavaScript.

### Undefined

A variable is undefined when it is declared but it has no value assigned to it yet.

```jsx
let children;
```

The variable exists and can be used. It can store a number, a boolean value or a string, meanwhile it is **undefined.**

### Null

Null is similar to undefined but used in some other circumstances. It means **empty value**.

*there’s a bug in JavaScript. When using **typeof** in **null*** *it returns an Object. This error was never corrected for legacy code reasons.*

### Symbol (ES2015)

Value that is unique and cannot be changed (introduced in the ES2015) - Not useful for now.

### BigInt

Larger integers. Numbers that are to large to be represented by the number type.

> JavaScript has **dynamic typing**. It means that it is not necessary to determine the type of the variable you are going to use when declaring the variable. It is determined automatically. **Dynamic typing** also means that when the variable is resigned its type also changes.
**That’s why is so important to understand the difference between Value and Variable, because in JavaScript its the value that has a type and not the variable.**
> 

## <a id="let">Let, Const and Var</a>

### Let

Let and Const were declared in the ES6 (modern JavaScript).

**Let** is used to declare variables that can have its value changed during the program execution. Variables declared using let can be ***resigned**.* It can be very useful declaring the variables in the beginning of the code and assigning a value to it later.

### Const

**Const** keyword is used to declare variables that aren’t supposed to have its value changed during the program execution. 

**Const** keywords always need to have an assigned value to it. It can’t be initialized empty, otherwise a syntaxError will occur. 

> Use **const** to declare variable as default. Only use let when sure it will need to be resign later in the program.
> 

### Var

It is important to knowing the use of **var** for legacy reasons, but its use must be completely avoided. 

The keyword **var** allows a complete mutation of variables during the code execution that can lead to bugs.

## <a id="basic">Basic Operators</a>

Operator allows us to transform values or combine multiple values and do all kind of work with values. 

- **Mathematical operators (- , + , *, **, / , %)**

> Note: The + sign also can be used to concatenate strings.
> 
- **Assignment operators (=, +=, -=, ++, —)**
    - =, used to assign a value to a variable;
    - += used to resign the value of a variable with a sum operation
    - -=, used to resign the value of a variable with the minus operation;
    - ++, —, used to increase or decrease the value of a variable by 1.

 

- **Comparison operators (==, ===, >, <, ≥, ≤) - Used to provide boolean values.**
    - ==, used to compare values;
    - ===, used to compare values and types (used when more rigorously comparison is needed);
    - >, <, ≥, ≤, used to compare numbers values, checking the conditions;

## <a id="operator">Operator precedence</a>

JavaScript has a well defined order of operator precedence. For example, all the mathematical operators are executed before the comparison operators.

The code is read from left to right and when there’s more then one operator to be executed, the precedence order come to action.

All references to operator precedence in the link bellow.

[MDN Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence)

## <a id="stringAndTemplate">String and Template literals</a>

Template literals is a better way to concatenate strings without using the + sign creating a better line of code, more readable. 

```jsx
//conventional way
let firstName = 'Helton';
let lastName = 'Oliveira';

const heltonName = "Hi, my first name is" + firstName + "and my last name is" + lastName; 

//template strings
let firstName = 'Helton';
let lastName = 'Oliveira';

const heltoName = `Hi, my first name is ${firstName} and my last name is ${lastName};` 
```

As we can see, using `` we start and finish the template and and to concatenate with a variable we use `${}`

## <a id="ifElse">If/Else statements</a>

if else statements allows us to creating a conditional check on our code. It means some peace of our code will be executed only **if** the conditions is true. 

But if the condition is checked as false? Then we can use the **else** to run another block of code that attend our need.

```jsx
const age = 30;

if (age == 30){
	console.log(`my age is ${age}`)
} else {
	console.log(`my age is not ${age}`) 
} 
```

Else is not always necessary. We can use just the **if** check condition in some cases and JavaScript will continue running the code right after the if statement ends.

## <a id="typeConversion">Type Conversion and Coercion</a>

Learn type conversion is important because convert string to number, string to boolean and others is necessary all the time.

***Type conversion*** is when the conversion is made manually, on the other hand ***type coercion*** is when JavaScript automatically converts a type behind a scene for us.

### Type conversion

Sometimes we will need to make mathematical operations using received values as inputs, but some times these values comes as strings, so a mathematical operation will not work.

A string conversion to number must be done first using the JavaScript native function `Number()`.

```jsx
let birthYear = "1992"
let yearsOld = 30;

let actualYear = birthYear + yearsOld;
console.log(actualYear);
//the console above will print to the console >  199230

let actualYear = Number(birthYear) + yearsOld;
console.log(actualYear);
//Now using Number() the console will show as result > 2022

```

We can also do the same to convert numbers to strings using `String()`

### Type coercion

As already said, type coercion is an automatically conversion of typos by the JavaScript. 

We have as example the concatenation of a string and numbers. The final result will be a string.

```jsx
let age = 30;

console.log("My name is Helton and i am" + 30 + "years old")
//My name is Helton and i am 30 years old
```

A string will be printed to the console because the plus sign responsible for the concatenation tells to the JavaScript that there’s a number to be converted in a string.

In the other hand the minus sign trigger the opposite conversion, string to number, as we can see bellow.

```jsx
let birtYear = 1992;
let currentYear = "2022";

let age = currentYear - birtYear;
console.log(age);
//30
```

In the example above the minus sign triggered the string to number conversion and the string “2022” was converted to a number and the mathematical operation was completed.

The same will occur to the multiply ***** and the divide **/** operator.

## <a id="truthy">Truthy and Falsy values</a>

Falsy values are values that will become a false value when we try to convert them into a boolean value.

In JavaScript there are five falsy values and they are: **0**, **“”*(empty string)***, **undefined**, **null** and **NaN**. All these values will become ***false*** when converted to boolean even they’re not false initially.

```jsx
console.log(Boolean(0));
//the console will show 'false'
```

> `*Boolean() is a function similar to Number() and String() that are used to convert values in boolean values.*`
> 

Every value that not match with the description above are **Truthy** values, it means will become ***true*** when converted to boolean.

Otherwise in JavaScript the conversion to boolean values are always executed as **type coercion** in other words JavaScript do the job behind the scenes.

**But when exactly JavaScript do the type coercion to boolean? There’s two scenarios: *when using logical operators and in a conditional statement (if/else).***

```jsx
const money = 0;

if (money){ //money is covnerted to boolean using type coercion so the if/else conditional can check if the value is true of false. 
//In this case 0 is a falsy value that will produce a false boolean value when converted.
	console.log("Don't spend it all");
} else {
	console.log("You should get a job!")
}
//the message 'You should get a job' will be printed to the console as the result was a false boolean value, then the 'else' block that is going to be executed
```

## <a id="equality">Equality operators</a>

### loose equality operator (==)

Equality operators are used to check the equality of values. Using double equal signs (==) we can create conditional statements for example:

```jsx
let age = 18;

if (age == 18) console.log("You just became an adult");

//Note1: If statement using an equality operator that results in a true value (boolean value);
//Note2: JavaScript allows us to ignore the brackets when there's only one line of code to be executed inside the if statement.
```

### strict equality operator (===)

The main difference between strict operator and loose operator is that the strict operator does not perform the **type coercion.** But what does it means?

Well, type coercion is an action performed by the JavaScript (without user interference) that convert the type of a value before an action. Using a loose operator **(==)** the type coercion is allowed then we can have true results as boolean values even in case as the example below:

```jsx
if ('18' == 18) console.log("They are equal");

//the console will print the message because the type coercion will occur and transform the '18' (string) in a 18 (number) so the boolean value returned in the comparison will be 'true'.
```

Using the same example above but with a strict equality operator we can see the difference:

```jsx
if ('18' === 18) {
	console.log("They are equal");
} else {
	console.log("They are different");
}

//the console will print 'They are different' once the type coercion will note occur then the conversion of the 18 (string) to 18 (number) will never happen. 
```

### Different operator (!= / !==)

Different operator check if a condition is false then run the code. It is very similar to the equality operator having also a loose and strict mode.

 

```jsx
const bestColor = 'blue';

if (bestColor !== 'red') console.log("Why not red?");
//The console will print the message 'Why not red' because the bestColor is different than Red.
```

## <a id="boolean">Boolean Logic (true or false)</a>

Boolean logic is a branch of computer science that uses True of False values to solve logical problems.

3 operators are used in Boolean Logic, AND (&&) operator, OR (||) operator and NOT (!) operator. Using these operators we can combine results of differente conditions to run or not run our code.

AND operator will only run the code if every statement in the conditional check were true. The OR operator needs only one statement as true to run the code, even if the other were false. The NOT operator turns the statement true in false and vice versa. 

> AND = if at least one of the values is false, the result of the conditional check will be false.
OR = if t least one of the values is true, the result of the conditional check will be true.
> 

![Untitled](The%20Complete%20JavaScript%20Course%20b30eb897e777483da96dbcceccb008bd/Untitled.png)

## <a id="logical">Logical Operators (&&, ||, !)</a>

We can use boolean values and logical operators to model complex situations.

```jsx
const hasDriverLicense = true;
const hasGoodVision = true;

if(hasDriverLicense && hasGoodVision) {
	console.log('Sarah is able to drive');
} else {
	console.log('Sarah is not able to drive');
}

const isTired = true;

if (hasDriverLicense && hasGoodVision && !isTired) {
	console.log('Sarah is able to drive');
} else {
	console.log('Sarah is not able to drive');
}
```

## <a id="switch">The Switch statement</a>

The switch statement is a toll to compare a value with multiple options.

```jsx
const day = 'monday';

switch(day) {
	case 'monday':
		console.log('Plan a course');
		console.log('Coding meetup');
		break;
	case 'tuesday':
		console.log('Prepare theory videos');
		break;
	case 'wednesday':
	case 'thursday':
		console.log('Record videos');
		break;
	case 'friday':
		console.log('Write code examples');
		break;
	case 'saturday':
	case 'sunday':
		console.log('Enjoy the weekend');
		break;
	default:
		console.log('Not a valid day');
}
```

The switch statement execute a **strict comparison.** It is very similar to a If/Else statement. Although the switch statement is more  and more less used, it can be very helpful in comparison situations where a if/else statement produces a repetitive code and the switch statement being more readable.

## <a id="statements">Statements and Expressions

### Expression

Expression is a peace of code that produces a value, for example:

```jsx
const n = 3 * 4;
//3 * 4 is a expression that produce a value
1991
//1991 is also a expression because in the end it has produced a value
true && false && !false
//An expression as well once it produce a value.
```

### Statement

Statements are a big peace of code and which does not produce a value on itself. Creating a program is to create a sequence of actions and these actions are the statements.

```jsx
if (23 > 10) {
	const n = '23 is bigger than 10';
}
```

The if statement above has performed an action but not produced a value. It just has stored the string in a variable.

Is important to know the difference between both but it gets more natural along the time.

For example, Template literals always awaits for expressions and not statements. We can’t insert a statement in a template literal. 

```jsx
console.log(`I'm ${2022 - 1992} years old`);
//There's a expression inside the ${}.
```

## <a id="conditional">The Conditional (Ternary) Operator</a>

The ternary operator allow us to create if/else statements using only one line of code.

```jsx
const age = 23;
age >= 18 ? console.log('I like to drink wine') : console.log('I like to drink water');
```

The ternary operator is called that way because it is composed by three parts, first the conditional statement check the finish in the interrogation mark, the second part is the block that is going to be executed in case the condition checked is true, the second block ends in the colon. And the third block is the else block that will be executed in case the conditional check is false.

The best part is that the Ternary operator as the name is said is an Operator, and as an operator it produces a value.

So, basically we transform the if/else from a statement in an expression, this way we can store a value produced by the block of code.

Ternary operators are a good way to declare variables after a condition check.

```jsx
const age = 23;

const drink = age >= 18 ? 'wine' : 'water';
console.log(drink);
//Will print 'wine'
```

Another big advantage to use ternary operator is to combine it with template literals. As we already saw, template literals just accept expressions, so it is impossible to insert an if/else statent in it, unless we use the ternary operator:

```jsx
console.log(`I'd like to drink ${age >= 18 ? 'wine' : 'water'}`);
```

## <a id="activate">Activate Strict Mode</a>

The **strict mode** is a special mode that we can activate to write a secure JavaScript code. 

```jsx
'use strict'

//code start bellow
```

To activate the strict mode is necessary just to write the string ‘use strict’ in the first beginning of the program.

Is also possible to activate a strict mode for a specific function using the string ‘use strict’ right before the function (but is not the better use for it).

The strict mode help developers avoid create bugs in the code, and that’s because of 2 reasons:

- Forbid us to do certain things;
- Create visible errors for us in certain situations in which some situations JavaScript will fail silently without letting us know that we did a mistake.

## <a id="functions">Functions</a>

What is a function? A function is a peace of code that we can reuse during the program execution. We can use this piece of code over and over always when necessary.

It is very similar to a variable, but for a whole bunch of code.

> **Remember that a variable is like a box where we can store a value. Functions are boxes where we can store statements and lines and more lines of code.**
> 

```jsx
//structure of a function

function logger() {}

//start with the keyword ***function***
//followed by the name of the function (***logger*** in this example)
//parentesis to determine if the function will receive a external value to work with (parameter)
//curlibraces where the function code will be written

logger();
//this short line of code above calls the function.
//A function will only be executed if we call it somewhere in the code
//the structure that calls a function is the name of the function followed by the parentesis
//the parentesis can be empty or with a value the will be passed into the function
```

```jsx
function logger() {
	console.log('My name is Helton');
}

logger();
logger();

//this block of code above will print to the console 'My name is Helton' twice.
```

**Function can also receive data and return data back**

When calling a function we saw before an empty parentheses, but a function can receive a data and work with it. Using the same example:

```jsx
function logger(name) {
	console.log(`My name is ${name}`);
}

logger('Helton');
logger('Laiz');

//Same function but now producing different results for each time the function is called.
//The first time the function is called it will print to the console 'My name is Helton'
//The second 'My name is Laiz'
```

The main difference is that when create the body of the function we set a **parameter** inside the parentheses, in this case we used ‘name’. This tell to the program that our function will receive a value when called. The **parameter** becomes a variable inside the function that will store the value passed and it can be used as wished inside the function. 

In our example the ***name*** is the name of the parameter defined during the creation of the function. Inside the function **name** will be a variable that has stored the value passed when the function was called.

When we first called our function, now knowing that we need to pass a value to attend the parameter, we have passed the string ***‘Helton’*** as a value. This string will be stored in the ***name*** inside the function.

The last step was to console our message using our variable to print the name ***‘Helton’***

Right after that we called the same function, but now passing another string as value, that name ***‘Laiz’***. It works the same way changing only the name that was passed to the function. 

This is the main reason to use functions, we can repeat actions without repeating the code and when needed to produce different values we can send different information to attend the  ***function parameters.***

> **Parameters are the input data of a function - and it works like variables to be used only inside the functions**
> 

### Returning a value from a function

Let’s start with an example:

```jsx
function fruitProcessor(apples, oranges) {
	const juice = `Juice with ${apples} apples and ${oranges} oranges`;
	return juice;
}

const appleJuice = fruitProcessor(5, 0);
console.log(appleJuice);

const appleOrangeJuice = fruitProcessor(2, 4);
console.log(appleOrangeJuice);
```

Now that we know how parameters works, in other words, function input values, we are going to see the output values that we can obtain through the keyword ***return.***

In the exemple above we called a function and send to it the input values 5 and 0. In this case we have two scenarios:

 - a function that has two parameter (apples, oranges): In this case, these parameters are the empty variables that will receive the value from the function call and it will be possible to be used inside the function.

 - a function being invoked passing the arguments that will attend and be used by the parameters as a variable inside the function.

Long story short, when we create a function we must define the **parameters** of that function (if a parameter was necessary), in other words, we define what input values we expect to receive when this function is called. And when invoking a function we pass the **arguments** to that function. 

All that said we can back to the **return** and talk about the **output values.**

The action executed by the function can produce a value and this value can be used as an **output value** in other places inside the program, but for that we must use the keyword **return** to reference the value that we want to be the output value. In our example this value was the variable `juice`.

But how the output value works and how we can use this value?

A function has 3 phases, when it is called (before that the function is in a standby phase), when it is executing its action and when it finish its execution. In the last phase the function can become an variable to store a value and it happens when we use the keyword **return** to set the output value.

Looking to our example, our function `fruitProcessor` was in a stand by phase, then it was called and the values 5 and 0 was passed as arguments to attend the function parameters, then the function enters in its second phase, the execution phase. After it finish its execution a value was produced and stored in a variable called `juice`. At this point, the value stored in the variable `juice` only exists inside the function and can’t be used in other place outside the function. To solve this problem the keyword **return** was used and set the output value as the variable `juice` and this is the function third phase, now the function is a variable that store the value that once was in the variable `juice` and now this value can be used outside the function.

If we want to use this value more than one time is important to store this value in a new variable, for example:

```jsx
const appleJuice = fruitProcessor(5, 0);
```

Using just one line of code we called the function passing the arguments and assigned it to a new variable that will store the value returned by the function. After that, always when necessary to use the value returned by the function is just use the variable `appleJuice`.

## <a id="declaration">Function Declarations vs. Expressions</a>

### Function Declaration

In JavaScript there are different ways of writing functions and each type of function works in a different way (still similar though).

Until now we have used the **Function Declaration**, because of the ***function*** keyword to declare a function a bit like we declare a variable. 

```jsx
//function to calculate a person age
//remember that a parameter is like a local variable that only works in side the function.
function calcAge(birthYear) {
	//mathematical operation to find the age and store the value inside the variable 'age'
	age = 2022 - birthYear;
	//using the return with the variable 'age' so this way this value can be acessible outside the function.
	return age
}
```

We can improve this function writing it with less lines of code:

```jsx
function calcAge(birthYear){
//if the main objective of the function is to produce a value that will be used outside the function it isn't necessary to previously store the value in a variable, we can simply return the expression and the result value will be acessible outside the function.
//Remember that expressions are every line of code that produces a value, in this case our expression is the mathematical operation '2022 - birthYear'
	return 2022 - birtYear;
}

//invoking the function and passing the value 1992 as the argument to attend the parameter of the function.
//after the execution the produced value is acessible through the function and it can be stored in a variable
const age = calcAge(1992);
```

This is the **Function Declaration**, when we use the keyword ***function*** to create a function.

### Expressions (Anonymous Function)

In the past example create a function naming just after the keyword ***function***.

Also our last example as divided in three steps:

1 - create a function

2 - call the function

3 - store the returned value in a variable so we can continue using the produced value outside the function.

But if we can store a function in a variable?

For that we have what is called ***Anonymous Function***. Let’s see how it is structured:

```jsx
const calcAge = function(birthYear) {
	return 2022 - birthYear;
}

const age = calcAge(1992);
```

In an anonymous function is possible to assign a function to a variable, now the act of naming the function is no more needed because the function will assume the name of the variable that it was assigned to. 

 

```jsx
function calcAge(birthYear) {
	return 2022 - birthYear;
}

const age = calcAge(1992)

//transforming the function declaration in an Anonimous Function

const calcAge = function(birtYear){
	return 2022 - birthYear;
}

const age = calcAge(1992);
```

Anonymous functions are actually expressions and as all expressions produces (or are a) value it allows us to store it directly in a variable.

Even though both examples works in a similar way, is important to know both structures because in some cases it will be necessary to use **anonymous function**. 

### Real difference between Function Declarations and Function Expressions

The big deal between these two types of function is that we can call a **function declaration *before it is defined in the code***. 

In a **function expression *it will always necessary to define the function before calling  it***.

It is all correlated to a process called **hoisting** the we will see later, but for now is important to understand this main difference between ***function declaration and function expression.***

To use **function expressions** we can create a better structure of code, this way we will have everything stored in variables, values and functions and also using function expressions we will avoid the process of ***hoisting***.

## <a id="arrow">Arrow Functions</a>

Arrow function is a third way to write a function in JavaScript implemented in ES6. It is a shorter way and therefore faster to write.

It’s important to know that an Arrow Function is still a Function Expression. Let’s see the difference:

```jsx
//Anonymous function
const calcAge = function(birthYear) {
	return 2022 - birthYear;
}

//Arrow function
const calcAge = birthYear => 2022 - birthYear;
```

As we can see the arrow function is shorter because isn’t necessary to use the curly braces and the **return** happens implicitly. The result of the expressions written after the arrow `=>` will be automatically returned and stored in the variable that it is assigned to.

> **the arrow function structure above is used when the function has only one parameter and just one line of code to run.**
> 

**Let’s implement more lines of code.**

```jsx
const yearsUntilRetirement = birthYear => {
	const age = 2037 - birthYear;
	const retirement = 65 - age;
	return retirement;
}
```

Now the curly braces and the return has returned to the function.

There’s one more rule we must take a look. Until now we used only one parameter and for that reason wasn’t necessary to use the parentheses as it is used in normal functions, however there’s two scenarios where the parentheses must return and it happens when we don’t have any parameters (for that we will use an empty parentheses) or when we have two or more parameters. Let’s see an example:

```jsx
const yearsUntilRetirement = (birthYear, firstName) => {
	const age = 2037 - birthYear;
	const retirement = 65 - age;
	return `${firstName} retires in ${retirement} years`;
}

console.log(yearsUntilRetirement(1992, 'Helton'));
```

Last question to end this topic. **Should we always use arrow function?**

The answer is **NO!** 

When the code gets bigger, with multiple lines the advantage of use arrow function shrinks and the other reason is that arrow functions as we saw is a function expression and as a function expression it don’t get the keyword **this**.  (That is why is so important to understand the difference between a function declaration and a function expression). This topic will come back later in a more advanced content, for now i will let a link [***here***](https://www.codementor.io/@dariogarciamoya/understanding-this-in-javascript-with-arrow-functions-gcpjwfyuc) to read more about the **this** keyword in **arrow functions** 

## <a id="calling">Functions Calling other Functions</a>

Let’s start this topic with a very importante principle called **DRY (Don’t Repeat Yourself)**.

Functions calling other functions is the main pillar to create better code structure and as said above **Don’t Repeat Yourself.**

A program is a package of organized functions that when running can ‘talk’ to each other to achieve its main objective. A lot of functions inside a program would need to be executed multiple times, each time producing a differente value.

The DRY principle comes in handy to create these functions that will be executed multiple times, so this way we don’t need to repeat code. It is also useful to maintain the code once a change in the code is needed, the line of code to be changed will be easier to be found and modified.  

Long story short, let’s see how it works.

```jsx
function fuitProcessor(apples, oranges){
	const juice = `This juice was made with ${apples} apples and ${oranges} oranges`;
	return juice;
}

console.log(fruitProcessor(5, 3));
```

This function we’ve used before will be our example. In this function we made a Juice with a number of fruits passed as arguments when the function is called. Now we are going to improve this Juice Maker. Let’s consider that our processor is not so powerful and only process pieces of fruits, so before we make our juice we have to send our fruits to be cut into pieces. In this scenario we will call another function to cut our fruits, but this call will be made inside our main function, **fruitProcessor.** It will allow us to write less code. Time to see it:

 

```jsx
function fruitPieces(fruit){
	const fruitPiece = fruit * 4;
	return fruitPiece;
}

function fruitProcessor(apples, oranges){
	const applesPieces = fruitPieces(apples);
	const orangesPieces = fruitPieces(oranges);

	const juice = `This juice was made with ${applesPieces} apple pieces and ${orangesPieces} orange pieces`;
	return juice;
}

console.log(fruitProcessor(5, 2)); //Will print to the console "This juice was made with 20 apple pieces and 8 orange pieces";
```

As we can see the function **fruitProcessor** was responsible to call the other function **fruitPieces** sending the values received as arguments, then the function **fruitPieces** do its action and return the new value to the **fruitProcessor** function.

At first glimpse we can’t notice how it helps to write less code, so lets see how it would be written without a function calling the other function.

```jsx
const apple = 5;
const orange = 2;

function fruitPieces(fruit){
	const fruitPiece = fruit * 4;
}

const applePieces = fruitPieces(apple);
const orangePieces = fruitPieces(orange);

function fruitProcessor(apple, orange){
	const juice = `This juice was made with ${apple} apple pieces and ${orange} orange pieces`;
	return juice;
}

console.log(fruitProcessor(applePieces, orangePieces));

```

The code above will produce the same result as the last one, but its use is not even close to be considered in a real situation. The code was basically divided in two blocks, the first one where there’s the function to cut the fruits, for that we have variables being set, the function sctructure and the function call, only after that we will have our main function, the *juice maker*. 

To put an end point in this topic remember, **Don’t Repeat Yourself.** Let the code do the work that it can do for you, let it call the functions inside other functions, let the code talk to itself and have a good dialogue. This will help you find the bugs and kill them. Maintain your code is going to be a light work.

## <a id="reviewing">Reviewing Functions</a>

### Types of function that can be used

![Untitled](The%20Complete%20JavaScript%20Course%20b30eb897e777483da96dbcceccb008bd/Untitled%201.png)

### Anathomy of a function

![Untitled](The%20Complete%20JavaScript%20Course%20b30eb897e777483da96dbcceccb008bd/Untitled%202.png)

## <a id="arrays">Introduction to Arrays</a>

Remember this word: **Data Structure**. Data Structure are structures used in programming no matter what language do you work with. The first one we are going to talk about is called **Array.**

**Arrays** are like a big container where we can throw variables and reference them before.

We use variables to store values and information, but in some cases we are going to work with values that has a connection to each other, or has something in commom, or belong to a certain group. Creating a variable to each value can violate our DRY principle after all we will have to create as many variables as necessary to store all values that we need to be stored and to use these variables in the program we will have to call them by name. See how can it be suscesptible to errors and bugs? But how to fix it using Arrays and how actually Arrays works?

**Arrays** works as a variable that can store more then one value in a indexed way. 

Let’s consider we have a list of friends to call to our birthday party:

```jsx
const friend1 = 'João';
const friend2 = 'Maria';
const friend3 = 'Jose';
```

This is so tiring, but the Array came to our save:

```jsx
const friends = ['João', 'Maria', 'Jose'];
//we create arrays by setting the values inside brackets separated by comma.
//Note that we create an array of strings, but arrays can store all types os values, as strings, numbers, booleans, etc.

//There's another way to create arrays, but it is not as usual as the first example.
//We can also create arrays using the keyword 'new' followed by the JavaScript native function 'Array', for example:
const friends = new Array('João', 'Maria', 'Jose');
```

The first option we used only pure code, that we can call **Data,** to store our values, but in the second example we used our first **data structure**. It allows us to obtain the same result using less code. Not only using less code, but using Arrays we can create a cleaner and organized code. 

Until now we have only talked about of inserting data in an **Array**, but how can we retrieve these values?

First and one of most important information about Arrays is that arrays has a zero based index, remember that, because to retrieve the correct values we must understand what zero based index is.

Now we can see a code example:

```jsx
const friends = ['João', 'Maria', 'Jose'];
//Zero based index means that the first value stored in the arrays is in the position 0.
//friends[0] = 'João';
```

To retrieve the first value of an array we must use **0**. And if the array has 3 values stored in it, the last one will be stored in the position **2.** Never mix up quantity of values stored in an array with position of its values. 

To help us understand we will use an **array property** called ***length.*** 

After a creation of an array we can use the ***length*** property to discover how many values are stored in our array:

```jsx
const friends = ['João', 'Maria', 'Jose'];
console.log(friends.length); //will print to the console the value '3';
```

The ***length*** property can also help us to retrieve the last element of our array even if we don’t know how many elements our array has.

```jsx
const friends = ['João', 'Maria', 'Jose'];
console.log(friends[friends.length - 1]); //will print 'Jose' to the console.
```

It is obvious that you have noticed the subtraction operation realized inside the brackets. We know that the ***length*** property will return for us the number 3 that is the amount of elements in our array, but when we are retrieving values from our array we use the index value of the element, and as array is zero based our exemple doesn’t have an index of value 3, it ends in the index of value 2 (0 for João, 1 for Maria and 2 for Jose). *It lead us to set the **length - 1** operation will always return for us the last element of the array, **because the result of these operation will be a value equal to the last index value of the array.***

Another important information is that ***JavaScript accept expressions inside the brackets when retrieving an array element.*** Remember, expressions are line of code that has a value as a result. 

Let’s practice to improve our understanding:

We will create a function that retrieve values from an array and return it to a new array

```jsx
const birthYear = [1996, 2004, 2016, 2018]

function calcAge(birthYear){
	const age = 2050 - birthYear;
}

const ages = [calcAge(birthYear[0]), calcAge(birthYear[1]), calcAge(birthYear[2]), calcAge(birthYear[3])]
```

> Using ***const*** to declare arrays forbid us to reassign an entire array, but still allow us to change the elements inside the array, because the **const keyword** only forbid changes in JavaScript primitive values and array elements aren’t primitive values.
> 

```jsx
//This is forbidden and will throw an error
const age = [10, 25, 43];
age = [15, 46, 56]
//In the code above we are reassign an intire array into the same variable (age) that store it

//It is allowed
const age = [10, 25, 43];
const age[0] = 15;
//The code above change the value inside the array without changing the array structure that are already stored in the variable age.

//imagine that the variable age is a container that store a small container with 3 numbers inside it, in the first example we try to remove the whole small container from inside the age container to put a new small container.
//In the second example, the small container inside the container age remains the same, we just open the container age, open the small container and change the value inside it.
```

## <a id="basicArray">Basic Array Operations(Methods)</a>

There are countless array methods in JavaScript, they are very important and we will learn all of them before, but for now we are going to learn some basic ones to get used of using methods in JavaScript.

One note before we start. **Methods** are technically a function. They are represented by the name of the method followed by parentheses, so calling methods in arrays is like calling a function to execute some action to that array.

> ***Methods can be also used in others Data Structures, like Objects. Although there are different methods for different data structure the principle of a method will always remain the same.***
> 

### Push

Push will be the first method we will learn. **Push** method adds elements to the end of an array and it can be called using the syntax `array.*push()`* with the element to be add to the array written inside the parentheses.

```jsx
const friends = ['João', 'Maria', 'José'];
console.log(friends); //will print to the console: ['João', 'Maria', 'José']

friends.push('Jorge');
console.log(friends); //will print to the console: ['João', 'Maria', 'José', 'Jorge'];
```

Knowing that **methods** are in fact functions, so the ‘Jorge’ in the example above is the ***argument*** passed to the method/function. Also as a function, the push method can return a value and this value is the new length of the array. We can store this value in a new variable if its use will be needed before in the code.

```jsx
const friends = ['João', 'Maria', 'José'];
const newLength = friends.push('Jorge');
console.log(newLength); //will print to the console the value ***4*** because after performing the action of adding 'Jorge' to the array friends, the function/method push return the new length of the array that now is 4 and it was assigned to a new variable called ***newLength***.
```

### Unshift

To save time we are going to say only that ***unshift*** perform the same action of ***push*** that is to add elements to the array***.*** **Unshift** add new elements to the array, in the beginning of the array though.

```jsx
const friends = ['João', 'Maria', 'José'];
console.log(friends); //will print to the console: ['João', 'Maria', 'José']

friends.unshift('Jorge');
console.log(friends); //will print to the console: ['Jorge', 'João', 'Maria', 'José'];
```

***unshift also returns the value of the new length of the array***

### Pop

As we can add elements to an array we can also remove elements from it. **Pop** is a method that removes the last element of an array.  

```jsx
const friends = ['João', 'Maria', 'José'];
console.log(friends); //will print to the console: ['João', 'Maria', 'José']

friends.pop();
console.log(friends); //will print to the console: ['João', 'Maria'];
```

The **pop** method syntax is slightly different, when using **pop** we won’t pass any arguments. The parentheses will be empty.

There is another difference and it is in the returned value. The last two methods, *push* and *unshift* return the new length of the array meanwhile the **pop** method returns the removed element.

```jsx
const friends = ['João', 'Maria', 'José'];
console.log(friends); //will print to the console: ['João', 'Maria', 'José']

const poppedElement = friends.pop();
console.log(friends); //will print to the console: ['João', 'Maria'];
console.log(poppedElement); //will print to the console: 'José';
```

### Shift

Just as **unshift** is to **push**, **shift** is to **pop.** Meanwhile **pop** removes the last element of the array, **shift** removes the first.

Both also have the similarity when talk about the returned value. **Shift** will return the value that was removed.

```jsx
const friends = ['João', 'Maria', 'José'];
console.log(friends); //will print to the console: ['João', 'Maria', 'José']

const poppedElement = friends.shift();
console.log(friends); //will print to the console: ['Maria', 'José'];
console.log(poppedElement); //will print to the console: 'João';
```

### IndexOf

IndexOf is a method that return the index value of the element inside the array. The **IndexOf** syntax demands an argument to perform the check. If there is a value inside the array that is strict equal to the value passed as argument the method will return the index value where the element is stored.

```jsx
const friends = ['João', 'Maria', 'José'];
console.log(friends); //will print to the console: ['João', 'Maria', 'José']

const indexElement = friends.indexOf('Maria');
console.log(friends); //will print to the console: ['João', 'Maria', 'José'];
console.log(indexElement); //will print to the console: '1';
```

In case of search of elements that aren’t in the array, ***IndexOf*** will return ***-1***

### Includes

Very similar to ***IndexOf*** more more modern and more useful, Includes instead of returning the index of the element it returns a Boolean value (true or false), in other words it tells us if the value is in the array or not. 

Important to know that ***Includes*** uses strict equality, so if you has a number stored as string and search for it as a number it will return false.

```jsx
const friends = ['João', 'Maria', 'José'];
console.log(friends); //will print to the console: ['João', 'Maria', 'José']

const element = friends.includes('Maria');
console.log(element); //will print to the console: 'true';

const numbers = ['05', '15', '24'];
console.log(numbers); will print to the console: ['05', '15', '24']

const trueOrFalse = numbers.includes(24);
console.log(trueOrFalse); //will print to the console: 'false'; 
```

One of greatest use for ***includes*** is in conditional statements. It can help us reduce our code and it is very simple as we can see bellow:

```jsx
const friends = ['João', 'Maria', 'José']

if(friends.includes('Maria') {
	console.log('You have a friend called Maria');
}
//the statement above will print the message to the console once there's a value as string named 'Maria' inside the array.

if(friends.includes('Marcos') {
	console.log('This friend was invited to your birthday party');
} else {
	console.log('This person is a stranger');
}
//the statement above will print to the console 'This person is a stranger', because there isn't a value as string named 'Marcos' in the array.
```

## <a id="objects">Introduction to Objects</a>

**Object** is the second ***Data Structure*** we are going to learn.

Let’s do a recap in Arrays looking to it in a different way:

```jsx
const heltonArray = [
	'Helton',
	'Oliveira',
	2022 - 1992,
	'engineer',
	['Luiz', 'Helena']
];
```

The array above is structured in a different way, the elements are organized vertically. As we can see, an array can store multiples types of data, a string, number and even another array. Looking to an array structured like that will familiarize us with an Object structure.

Intuitively looking for this array we know that, in a descendent order we have a first name, last name, date of birth, profession and friends names, however it is not directly clear in the array what they are.

Using arrays we don’t have a way to name these elements, only reference them by its index value. To solve this problem JavaScript have the Data Structure called **Objects.**

Using **Objects** we can define key value pairs. And so then we can give each of these array elements a name.

We have some steps to follow to create an Object:

1. Create a variable to store the object;
2. Start the object structure using curly braces;
    1. An array structure starts and ends using brackets `[]`, when using objects, it is opened and closed using curly braces `{}`.
3. Define the key values that are basically the name of the variables;
4. Always remember to separate the values with comma like in an array.

Let’s create our fisrt Object using the past example:

```jsx
const helton = {
	fisrtName: 'Helton',
	lastName: 'Oliveira',
	age: 2022-1992,
	job: 'Engineer',
	friends: ['Luiz', 'Helena']
};
```

*The keys are also called **PROPERTIES**. So we can say that the array above has five properties. It is really important to remember because it is **the main difference between arrays and objects, meanwhile values in arrays are retrieved by its index, values in objects are retrieved using its properties (or key names) it means that using objects the order of these values does not matter at all when we want to retrieve them. We must keep it in mind when thinking about using arrays or objects, once arrays values only can be retrieved by its index values so the order of the values insed the array matters a lot. It means we should use ARRAYS for mor more order data and OBJECTS for more unstructured data and data that we want to name and retrieve from the object, based on that name.***

> **Objects** are probably the most important structure in JavaScript, so there’s many ways of creating it. The example above is the simplest way to create an object and it is called the ***object literal syntax (because we are writing down the whole object content***.
> 

To finish our introduction ***we use objects to group together variables that really belongs together, like properties of an object in a real world. And other big difference is that using objects the order of these values does not matter at all when we want to retrieve them.***

## <a id="dot">Dot vs Bracket Notation</a>

In this section we are going to learn how to retrieve and change data using **Dot** and **Bracket Notation.**