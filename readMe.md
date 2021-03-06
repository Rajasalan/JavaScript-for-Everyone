# JavaScript for Everyone
![JS](https://cdn-images-1.medium.com/max/1600/1*H-25KB7EbSHjv70HXrdl6w.png)
## Table of Contents
1. [Introduction](#introduction)
2. [Setup](#setup)
3. [Variables](#variables)
4. [Data Types](#data-types)
5. [Operators](#operators)
6. [Conditionals](#conditionals)
7. [Arrays](#arrays)
8. [Loops](#loops)
9. [Functions](#functions)
10. [Scope](#scope)
11. [Hoisting](#Hoisting)
12. [Object](#object)
13. [Class](#class)
14. [Document Object Model](#dom)
15. [Functional Programming](#functional-programming)
16. [Call Back and Higher Order Functions](#callback-and-higher-order-functions)
17. [Destructuring](#destructuring)
19. [Rest and Spread](#rest-and-spread)
20. [Document Object Model](#document-object-model)
21. [Regular Expressions](#regular-expressions)
22. [LocalStorage](#localstorage)
23. [Cookies](#cookies)

## Introduction
Welcome to JavaScript. ***Congratulations*** for deciding to learn JavaScript.
***JavaScript for Everone*** is a guide for both beginner and advanced JavaScript developers. In this step by step tutorial, I will teach you JavaScript, the most popular programming language in the history of mankind. You use JavaScript ***to add interactivity to websites, to develop mobile apps, desktop applications, games*** and nowadays JavaScript can be used for ***machine learning*** and ***AI***.
***JavaScript (JS)*** has increased in popularity in recent years and has been the leading
programming language for four consecutive years and is the most used programming language on
Github 
## Setup
First thing first, lets install text or code editor. Install code editor, it could be [vscode](https://code.visualstudio.com/), [atom](https://atom.io/), [bracket](http://brackets.io/), [notepad++](https://notepad-plus-plus.org/) or others. I recommend vscode.
## Adding JavaScript to a web page
JavaScript can be added to a web pages in three ways:
* ***Inline script***
* ***Internal script***
* ***External script***

The following sections shows different ways of adding JavaScript code to your web page.
### Inline Script
Create a folder on your desktop or in any location and create an ***index.html*** file. Then paste the following code and open it in a browser, either in [Chrome](https://www.google.com/chrome/) or [Firefox](https://www.mozilla.org/en-US/firefox/new/?v=b).

```html
<DOCTYPE html>
<html>
  <head>
    <title>JavaScript for Everyone</title>
  </head>
  <body>
        <button onclick= "alert('Welcome to JavaScript!');">Click Me</button>
  </body>
</html>
```
### Internal script
Internal script can be written in the ***head*** or the ***body*** but it is preferrable to put it on the ***body*** of the html document.
```html
<DOCTYPE html>
<html>
  <head>
    <title>JavaScript for Everyone</title>
  </head>
  <body>
   <script>
     console.log('Welcome to JavaScript for Everyone')
    </script>
  </body>
</html>
```
### External script
```html
<DOCTYPE html>
<html>
  <head>
    <title>JavaScript for Everyone</title>
  </head>
  <body>
  //it could be in header or in the body
  // Here is the recommended place to put the script
  <script src="script.js"></script>
  </body>
</html>
```
#### Exercises:Setting Up your machine
## Variables
Variables are ***containers*** of data. Variables ***store*** data in a memory location. When a variable is declared a memory location is reserved and when it is assigned to a value, the memory space will be filled. To declare a variable we use, ***var***, ***let*** or ***const*** key word. For a variable which changes at different time we use ***let*** but if the data doesn't change at all we use ***const***. For example PI, country name, gravity.
```js
// Declaring different variables of different data types
let firstName = "Asabeneh";
let lastName = "Yetayeh";
let location = "Helsinki";
const country = "Finland";
let age = 100;
let isMarried = true;
const gravity = 9.81;
const boilingPoint = 100;
const PI = 3.14;
console.log(firstName, lastName, location, country, age, gravity, PI);
// Variables can also be declaring in one line
let name = "Asabeneh",
  job = "Teacher",
  live = "Finland";
  console.log(name, job, live) 
```
#### Exercises:Variables
1. Declare variables to store your first name, last name,  marital status, country and age in multiple lines
1. Declare variables to store your first name, last name,  marital status, country and age in a single line
1. Declare two variables *myAge* and *yourAge* and assign them initial values and log to browser console. 
Output:
```sh
I am 25 years old.
You are 30 years old.
```

## Comments
Commenting in JavaScript is similar to other programming languages. Comments can help to make code more readable.
There are two ways of commenting:
* *Single line commenting*
* *Multiline commenting*
```js
    // let firstName = 'Asabeneh'; single line comment
    // let lastName = 'Yetayeh'; single line comment
```
Multiline commenting:
```js
    /*
    let location = 'Helsinki';
    let age = 100;
    let isMarried = true;
    This is a Multiple line comment
    */
```
#### Exercises:Comments
 
## Data Types
In JavaScript and also other programming languages there are different kinds of data types. The following are JavaScript primitive data types:***String, Number, Boolean, undefined, Null*** and ***Symbol***.
### Strings
Strings are text which are under ***single*** or ***double*** quote.
Lets' see some examples of string:
```js
let firstName = 'Asabeneh'
let country = 'Finland'
let city = 'Helsinki'
let language = 'JavaScript'
```
#### Exercises:String
1. Declare a variable name company and assign it to an initial value "Coding Academy".
1. Print the string  on the browser console using console.log()
1. Print the length of the string  on the browser console using console.log()
1. Change all the string to capital letters using toUpperCase() method
1. Change all the string to small letters using toLowerCase() method
1. Cut(slice) out the first word of the string using slice, substr() or substring() method
1. Check if the string contains a word Academy using includes() method
1. Split the string into array using split() method
1. Split the string Coding Academy at the space using split() method
1. "Facebook, Google, Microsoft, Apple, IBM,Oracle, Amazon" split the string at the comma  and change it to an array.
1. Change Coding Academy  to Microsoft Academy using replace() method.
1. What is character at index 10 in "Coding Academy" string use charAt() method.
1. What is the character code of A in "Coding Academy" string using charCodeAt()
1. Use indexOf to determine the position of  the first occurrence of e in Coding Academy
1. Use lastIndexOf to determine the position of the last occurrence of e in Coding Academy
1. Use trim() to remove if there is trailing whitespace at the beginning and the end of a string.E.g "  Coding Academy   ". 
1. Use startsWith() method with the string Coding Academy make the result true
1. Use endsWith() method with the string Coding Academy make the result true
1. Use  match() method to find all the a’s in Coding Academy
1. Use concat() and merge ‘Coding’ and "Academy" to a single string, "Coding Academy"
1. Use repeat() method to print Coding Academy 5 times

### Numbers
Numbers are integers and decimal numbers which can do all the arithemtic operators.
Lets' see some examples of Numbers
```js
let age = 35;
let gravity = 9.81;
let pi = 3.14;
let temperature = 37;

```
### Booleans
```js
let isRaining = false
let hungery = false;
let isMarried = true;

```
#### Exercises:Booleans
Boolean value is either true or false. 
1. Write three JavaScript statement which provide truthy value. 
1. Write three JavaScript statement which provide falsy value.
1. Boolean value is either true or false. Any comparison return a boolean either true or false. 
1. Use all the following comparison operators to compare the following values: >, < >=, <=, !=, !==,===. 
Which are true or which are false ?
  1. 4 > 3
  1. 4 >= 3
  1. 4 < 3
  1. 4 <= 3
  1. 4 == 4
  1. 4 === 4
  1. 4 != 4
  1. 4 !== 4
  1. 4 != '4'
  1. 4 == '4'
  1. 4 === '4'

### Undefined
```js
let firstName;
console.log(firstName); //not defined
```
### Null
```js
let empty = null;
console.log(empty); //no value
```
#### Exercises:Data types
String, number, boolean, null, undefined and symbol(ES6) are JavaScript primitive data types.
- The JavaScript typeof operator uses to check different data types. Check the data type of each variables from question number 1.

## Operators
### Arthimetic Operators
```js
let numOne = 4;
let numTwo = 3;
let sum = numOne + numTwo;
let diff = numOne - numTwo;
let mult = numOne * numTwo;
let div = numOne / numTwo;
let remainder = numOne % numTwo;

```
#### Exercises:Arthimetic Operators:
JavaScript arithmetic operators are addition(+), subtraction(-), multiplication(*), division(/), modulus(%), increment(++) and decrement(--).
```js
let operandOne = 4;
let operandTwo = 3;
```
Using the above operands apply different JavaScript arithmetic operators

### Logical Operators
&& , ||

```js
const check = 4 > 3 && 10 < 5;
const check = 4 > 3 || 10 < 5;

```
#### Exercises: Logical Operators
Which are true or which are false ?
1. 4 > 3 && 10 < 12
1. 4 > 3 && 10 > 12
1. 4 > 3 || 10 < 12
1. 4 > 3 || 10 > 12
1. !(4 > 3)
1. !(4 < 3)
1. !(false)
1. !(4 > 3 && 10 < 12)
1. !(4 > 3 && 10 > 12)
1. !(4 ===’4’)

### Comparison Operators

```js
4 > 3;
4 >= 4;
4< 3
4 <= 3
4 === 4
4 !=3;
4 !== '4';
4 !=== '4'
4 == '4'
4 === '4'
```
#### Exercises:Comparison Operators
Boolean value is either true or false. Any comparison return a boolean either true or false. 
Use all the following comparison operators to compare the following values: >, < >=, <=, !=, !==,===. 
Which are true or which are false ?
1. 4 > 3
1. 4 >= 3
1. 4 < 3
1. 4 <= 3
1. 4 == 4
1. 4 === 4
1. 4 != 4
1. 4 !== 4
1. 4 != '4'
1. 4 == '4'
1. 4 === '4'

## Arrays
In contrast to variables array can store *multiple values*. Each value in an array has an *index* and each index has *a reference in a memory address*. Each value can be accessed by using their *indexes*. The index of an array starts from *zero* and the last element is less by one from the lenght of the array.
```js
const webTechs = [
  "HTML",
  "CSS",
  "JavaScript",
  "React",
  "Redux",
  "Node",
  "MongoDB"
];
const countries = [
  "Albania",
  "Bolivia",
  "Canada",
  "Denmark",
  "Ethiopia",
  "Finland",
  "Germany",
  "Hungary"
];
const numbers = [0, 3.14, 9.81, 37, 98.6, 100];
const shoppingCart = [
  "Milk",
  "Mango",
  "Tomato",
  "Potato",
  "Avocado",
  "Meat",
  "Eggs",
  "Sugar"
];
console.log(webTechs);
console.log(webTechs.length) // => to know the size of the array, which is 7
console.log(webTechs[0]) //--> HTML;
console.log(webTechs[webTechs.length-1]) //--> MongoDB
console.log(countries);
console.log(numbers);
console.log(shoppingCart)

```
#### Exercises:Arrays
1. Declare an array  variable name itCompanies and assign initial values Facebook, Google, Microsoft, Apple, IBM, Oracle and Amazon.
1. Print the array using console.log()
1. Print the number of companies in the array
1. Print out each company
1. Change companies to uppercase and print them out
1. Print the array like as a sentence: Facebook, Google, Microsoft, Apple, IBM,Oracle and Amazon are big IT companies.
1. Sort the array using sort() method
1. Reverse the array using reverse() method

## Conditionals
#### If
```js
if(condition){
  //code goes here
}
let isRaining = true;
if (isRaining) {
  console.log("Remember to take your rain coat.");
}
```
#### If Else
```js
if(condition){
  // if the condition met

} else{
 // if condition doesn't met
}
let isRaining = true;
if (isRaining) {
  console.log ('You need a rain coat.');
} else {
  console.log ('No need for a rain coat.');
}
```
#### If Else if else
```js
// if else if else
let weather = 'sunny';
if (weather === "rainy") {
  console.log("You need a rain coat.");
} else if (weather === "cloudy") {
  console.log("It might be cold, you need a jacket.");
} else if (weather === "sunny") {
  console.log("Go out freely.");
} else {
  console.log("No need for rain coat.");
}
```
#### Switch
Switch an alternative for if else if else
```js
var weather = "cloudy";
switch (weather) {
  case "rainy":
    console.log("You need a rain coat.");
    break;
  case "cloudy":
    console.log("It might be cold, you need a jacket.");
    break;
  case "sunny":
    console.log("Go out freely.");
    break;
  default:
    console.log(" No need for rain coat.");
    break;
}
```
#### Ternary Operators
Another way to write conditionals is using ternary operators.
```js
let isRaining = true;
isRaining ?  console.log('You need a rain coat.') : console.log('No need for a rain coat.')

```
#### Exercises:Flow Control
- Get user input using prompt(“Enter your age:”). If user is 18 or older , give feedback:You are old enough to drive but if not 18 give feedback to wait for the years he supposed to wait for.
Output:
```sh
Enter your age: 30
You are old enough to drive. 
```

Output:
```sh
Enter your age:15
You are left with 3 years to drive.
``` 	
- Compare the values of myAge and yourAge using if … else. Based on the comparison log   to console who is older (me or you). Use prompt(“Enter your age:”) to get the age as input.
Output:
```sh
Enter your age: 30
You are 5 years older than me. 
```
```sh
let a = 4;
let b = 3;
```
- If a is greater than b return a is greater than b else a is less than b.
Output:
```sh
4 is greater than 3
```
## Loops
In programming languages to carry out repetitive tast we use different kinds of loop. The following examples are the commonly used loops.
### For Loop
```js
//For loop structure
for(initialization, condition, increment/decrement){
  // code goes here
}
for(let i = 0; i <= 5; i++){
  console.log(i)
}
 
```
### While loop
```js
let i = 0; 
while(i <= 5){
  console.log(i);
  i++;
}

```
### Do while loop
```js
let i = 0; 
do {
  console.log(i);
  i++;

} while (i <= 5)

```
#### Exercises:Loops
1. Iterate 0 to 10 using for loop, do the same using while and do while loop.
1. Iterate 10 to 0 using for loop, do the same using while and do while loop.
1. Iterate the array from above question using a for loop and print out the items.

## Functions
```js

function functionName(){
  // code goes here
}
functionName() // calling function

    // function without parameters
function addTwoNumbers() {
  var numOne = 10;
  var numTwo = 20;
  var sum = numOne + numTwo;
  console.log(sum);
}
addTwoNumbers(); // function has to be called to be executed
// Function without parater doesn' take input, so lets make a parameter with parameter
function sumTwoNumbers(numOne, numTwo) {
  var sum = numOne + numTwo;
  console.log(sum);
}
sumTwoNumbers(10, 20); // calling functions
// If a function doesn't return it doesn't store data, so it should return
function sumTwoNumbersAndReturn(numOne, numTwo) {
  var sum = numOne + numTwo;
  return sum;
}
console.log(sumTwoNumbersAndReturn(10, 20));
function printFullName(firstName, lastName) {
  return `${firstName} ${lastName}`;
}
console.log(printFullName("Asabeneh", "Yetayeh"));
console.log(printFullName("Dean", "Phan"));

function square(number) {
  return number * number;
}
console.log(square(10));

// this function takes array as a parameter and sum up the numbers in the array
function sumArrayValues(arr) {
  var sum = 0;
  for (var i = 0; i < arr.length; i++) {
    sum = sum + numbers[i];
  }
  return sum;
}
const numbers = [1, 2, 3, 4, 5];
console.log(sumArrayValues(numbers));
    //calling a function
    AddTwoNumbers(4,3)
    const areaOfCircle = (radius) => {
      let area = Math.PI * radius * radius;
      return area;
    }

```
#### Exercises:Functions
1. Declare a function fullName and it print out your full name.
1. Declare a function fullName and now it takes firstName, lastName as a parameter and it returns your full - name.
1. Declare a function addNumbers and it takes two two parameters and it returns sum.
1. Declare a function name printArray. It takes array as a parameter and it prints out each value of thearray.
1. Declare a function name reverseArray. It takes array as a parameter and it returns the reverse of the arra- (dont’ use method).
1. Declare a function name capitalizeArray. It takes array as a parameter and it returns  the - capitalizedarray. 
1. Declare a function name removeItem. It returns array after removing an item
1. Declare a function name addItem. It returns array after adding an item
1. Declare a function name sumOfNumbers. It takes a number parameter and it adds all the numbers in that range.
1. Declare a function name sumOfOdds. It takes a number parameter and it adds all the odd numbers in that - range.
1. Declare a function name sumOfEven. It takes a number parameter and it adds all the even numbers in that - range.
1. Declare a function name 	. It takes a number parameter and it counts number of evens and odds in the - number.
output:
```she
evensAndOdds(100);
The number of odds are 50.
The number of evens are 51.
```
- Declare a function name randomHexaNumberGenerator. When this function is called it generates  a random hexadecimal  number. The function return the hexadecimal number.
output:
```she
console.log(randomHexaNumberGenerator());
 '#ee33df'
console.log(randomHexaNumberGenerator());
'#28def10'
console.log(randomHexaNumberGenerator());
'#38eeda'
```
- Declare a function name userIdGenerator. When this function is called it generates seven character id. The function return the id.
Output:
```sh
console.log(userIdGenerator());
41XTDbE
```
- Modify question number n . Declare a function name userIdGeneratedByUser. It doesn’t take any parameter but it takes two inputs using prompt(). One of the input is the number of characters and the second input is the number of ids which are supposed to be generated. 
```sh
userIdGeneratedByUser()
"kcsy2
SMFYb
bWmeq
ZXOYh
2Rgxf
"
userIdGeneratedByUser()
"3RexwUqvqe
rVUY6dC1il
YCf88ZHuAf
7JhI6Mn063
mo3GYyH26O
"
userIdGeneratedByUser()
"1GCSgPLMaBAVQZ26
YD7eFwNQKNs7qXaT
ycArC5yrRupyG00S
UbGxOFI7UXSWAyKN
dIV0SSUTgAdKwStr
"
```
- Write a function name rgbColorGenerator and it generates rgb colors.
Output:
```sh
rgb(125,244,255)
```
- Write a function name displayDateTime  and it display in this format: 28/08/2018 04:08
- Use the new Date() object to get month, date, year, hour and minute.
Output:
```sh
28/08/2018 04:08
```
## Object
Everything can be an object and objects do have properties and properties have values.
```js

const person = {
  firstName:'Asabeneh',
  lastName:'Yetayeh',
  age:100,
  location:'Helsinki',
  skills:['HTML', 'CSS', 'JavaScript', 'React','Node','MongoDB', 'Python', 'D3.js']
  getFullName:function() {
    return `${this.firstName}${this.lastName}`
  }
}
person.nationality = 'Ethiopian'
person.live = 'Finland';

```
#### Exercises:Objects
- Create an object literal called personAccount. It has firstName, lastName, incomes, expenses properties and it has totalIncomes, totalExpenses, acountInfo,addIncome, addExpence and accountBalance methods. Incomes is a set of incomes and its description and the same for expenses. 

## Class
```js
class Person {
  constructor(firstName, lastName, age, location,skills){
    this.firstName = firstName;
    this.lastName = lastName;
    this.age = age;
    this.location = location;
    this.skills = skills;
  }
  getFull () {
    return `${this.firstName} ${this.lastName}`
  }
}
```
#### Exercises:Classes
## localStorage
Local storage is used to store data on the browser.
```js
let skills = [
  {teck:'HTML',level:10},
  {tech:'CSS', level:9},
  {tech:'JS',level:8},
  {tech:'React', level:9},
  {tech:'Redux',level:10},
  {tech:'Node',level:8},
  {tech:'MongoDB',level:8}
  ]

let skillJSON = JSON.stringify(skills)
localStorage.setItem('skills',skillJSON);
let skillsObj = JSON.parse(localStorage.getItem('skills'),undefined, 4)
console.log(skillsObj)
localStorage.clear()
```
## Exercises:Local Storage
## Cookies
#### Exercises:Cookies
## Document Object Model
HTML document is structured as a JavaScript Object. Every HTML element has a different properties which can help to manipulate it. It is possible get, create, append or remove HTML elements using JavaScript. Check the examples below.

### Getting Element
```js
let allTitle = document.getElementsByTagName('h1');
let allTitle = document.getElementsByClassName('title');
let firstTitle = document.getElementById('first-title');
let allDiv = document.querySelectorAll('div');
let span = document.querySelector('span');
let firstPara = document.querySelector('#first-para');
let allPara = document.querySelector('.para');

```
### Creating Element
```js
let title = document.createElement('h1');
let firstTitle = document.getElementById('first-title');

```
### Adding attribute
```js
let title = document.createElement('h1');
let firstTitle = document.getElementById('first-title');
title.setAttribut('class', 'title');
title.setAttribut('id', 'first-title')

```
### Adding Text conent
```js
let title = document.createElement('h1');
let firstTitle = document.getElementById('first-title');
title.textContent = 'JavaScript for Everyone';

```

### Adding style
```js
let title = document.createElement('h1');
let firstTitle = document.getElementById('first-title');
title.textContent = 'JavaScript for Everyone';
title.style.color = 'green';
```

### Appending to parent
```js
let title = document.createElement('h1');
let firstTitle = document.getElementById('first-title');
title.textContent = 'JavaScript for Everyone';
title.style.color = 'green';

document.body.appendChild(title)
```
### Event Listeners
```js
const button = document.querySelector('button');
button.addEventListener('click', (e) => {
  console.log(e.target)
})

```
#### Exercises:Document Object Model

## Regular Expressions
```js
let pattern  = /[A-Z][a-z]{3,12}/
let name = 'Asabeneh';
pattern.test(name)
//output:true
```
#### Exercises:Regular Expressions
- Calculate the total annual income of the person from the following text. ‘He earns 4000 euro from salary per month, 10000 euro annual bonus, 5500 euro online courses per month.’
## Functional Programming
- Declare a function called getStringLists which takes an array as a parameter  and then returns an array only with string items.
- Declare a function called categorizeCountries which returns an array of countries which have some common pattern(you find the countries array from slack).
- Declare a getFirstTenCountries function and return an array of ten countries
- Declare a getLastTenCountries function and return an array of ten countries
- Find out with which letter are there many countries
