# Javascript Cheat Sheet
I created this file while learning JavaScript

## Data Types
Undefined, null, boolean, string, symbol, number and object

## Variables

var = Used throughout the whole program

let = Only used in the scope where it's declared

const = Value can never change


## Compound Assignment
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
```

## Escape sequences in strings
```javascript
/*
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

## Assignment operators
```javascript
=  // Assign a value to a variable
+= // Adds the value
-= // subtracts the value 
*= // Multiplies a variable
/= // Divides a variable
%= // divides a variable and assigns the remainder to the variable
```
