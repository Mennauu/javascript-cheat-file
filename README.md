# Javascript Cheat Sheet
I created this file while learning JavaScript

## Data Types
```javascript
Undefined, null, boolean, string, symbol, number and object
```

## Variables
```javascript
var = Used throughout the whole program

let = Only used in the (block) scope where it is declared, can only be declared once

const = Value can never change (read-only)
```

## Escape sequences in strings
```javascript
Code  Output

\'    single quote
\"    double quote
//    backslack
\n    newline
\r    carriage return
\t    tab
\b    backspace
\f    form feed
```

## Concatenating Strings
```javascript
// Example one
var example = "I'm the best. " + "You're the worst."

var exampleFirst = "I'm the best. "
exampleFirst += "You're the worst."

// Example two
var name = "Menno"
var sentence = "My name is " + name + ", and i'm the best"
```

## Nested array
```javascript
var myArray = [['Menno', 23], ['Frans', 25]]
var MyData = myArray[0][1]

console.log(myData) // = 23
```

## Manipulate arrays
```javascript
// Example .push(): add element to ending of array
var myArray = ['Hello', 'Hey', 'Hoi']
myArray.push(['Hi', 'Yo'])

console.log(myArray) // = ['Hello', 'Hey', 'Hoi', 'Hi', 'Yo']

// Example .pop(): remove the last element
var myArray = ['Hello', 'Hey', 'Hoi']
var removedFromMyarray = myArray.pop()

console.log(myArray) // = ['Hello', 'Hey']
console.log(removedFromMyarray) // = ['Hoi']

// Example .shift(): remove the first element
var myArray = ['Hello', 'Hey', 'Hoi']
var removedFromMyarray = myArray.shift()

console.log(myArray) // = ['Hey', 'Hoi']
console.log(removedFromMyarray) // = ['Hello']


// Example .unshift(): add element to begin of array
var myArray = ['Hello', 'Hey', 'Hoi']
myArray.shift()
myArray.unshift("Yo")

console.log(myArray) // = ['Yo', 'Hey', 'Hoi']
```

## Function
```javascript
function substractingNumbers(a, b) {
  console.log(a - b)
}
substractingNumber(10, 5)
```

## Return value from function
```javascript
function substractingNumber(num) {
  return num - 7
}

console.log(substractingNumber(10)) // = 7
```

## Arrow function
```javascript
// Normal
var myConcat = function(arr1, arr2) {
  return arr1.concat(arr2)
}

// Arrow
var myConcat = (arr1, arr2) => arr1.concat(arr2)
```

## Assignment operators
```javascript
=  // Assign a value to a variable
+= // Adds the value
-= // subtracts the value 
*= // Multiplies a variable
/= // Divides a variable
%= // divides a variable and assigns the remainder to the variable
```

```javascript
var a = 50

// Addition
a = a + 12
a += 12

// Substraction
a = a - 12
a -= 12

// Multiplication
a = a * 12
a *= 12

// Division
a = a / 12
a /= 12

// Modulo
a = a % 12
a %= 12
```
## Comparison operators

```javascript
==	equal to
===	equal value and equal type
!=	not equal
!==	not equal value or not equal type
>	greater than
<	less than
>=	greater than or equal to
<=	less than or equal to
?	ternary operator
```

## Logical operators
```javascript
&&	and
||	or
!	not
```

```javascript 
function operators(val) {
    // if (val < 10) {
    //   return "Hello"
    // }

    // if (val > 20) {
    //   return "Hello"
    // }

    if (val < 10 || val > 20) {
      return "Hello"
    }

  return "Goodbye"
}

operators(15)
```

## Else if statement
```javascript
function ifElseInOrder(val) {
  if (val < 5) {
    return "Less than 5"
  } else if (val < 10) {
    return "Less than 10"
  } else {
    return "Greater than or equal to 10"
  }
}

console.log(ifElseInOrder(3)) // = Less than 5
```
## Switch statement
```javascript
function caseInSwitch(val) {
  var answer = ""
  switch(val) {
    case 1:
      answer = "alpha"
      break
    case 2:
      answer = "beta"
      break
    case 3:
      answer = "gamma"
      break
    case 4:
      answer = "delta"
      break
  }

  return answer
}

console.log(caseInSwitch(3)) // = gamma
```

```javascript
function switchofStuff(val) {
  var answer = ""
  switch(val) {
    case "a":
      answer = "apple"
      break
    case "b":
      answer = "bird"
      break
    case "c":
      answer = "cat"
      break 
    default: 
      answer = "stuff"
      break
 }

 return answer
}
```

## Objects
```javascript
var testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "nikes",
  "friends": []
}

var hatValue = testObj.hat // = ballcap

// add to object
testObj['moms'] = "Wendy"

// remove from object
delete testObj.hat
```

```javascript
// What if there is a space in the object name?
var testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
}

var entreeValue = testObj["an entree"] // = hamburger
```

## While loop
```javascript 
var myArray = []

var i = 0
while(i < 5) {
  myArray.push(i)
  i++
}

console.log(myArray) // = [0, 1, 2, 3, 4]
```

## For loop
```javascript
var myArray = []

for(var i = 1; i < 5; i++) {
  myArray.push(i)
}

console.log(myArray) // = [1, 2, 3, 4]
```

```javascript
// Iterate through an array
var myArray = [2, 3, 4, 5, 6]
var total = 0

for(var i = 0; i < myArray.length; i++) {
  total += myArray(i)
}
```

## Math
```javascript
Math.random   number between 0 and 1
Math.floor    Rounds down a number
```

## parseInt

Takes a string and returns it into an integer (number)

```javascript
function convertToInteger(str) {
  return parseInt(str)
}
convertToInteger("56")
```

## Ternary operator
```javascript
// condition ? statement-if-true : statement-if-false

function checkEqual(a, b) {
  return a == b ? true : false
}
```

```javascript
// Nested ternary operator

function checkSign(num) {
  return num > 0 ? "positive" : num < 0 ? "negative" : "zero"
}

console.log(checksign(10)) // = positive
```

## Map
For every element in the array, do something

```javascript
let doubled = arr.map(num => {
  return num * 2;
})
```

## ForEach
executes a provided function once for each array element
```javascript
arr.forEach((num, index) => {
  return arr[index] = num * 2;
})
```

## Destrucuting assignment to assign variables from objects
```javascript
var voxel = {
  x: 3.6,
  y: 7.4,
  z: 6.54
}

// old way
var x = voxel.x
var y = voxel.y
var z = voxel.z

// new way
const { x : a, y : b, z : c } = voxel
```
