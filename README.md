# TA-Lesson

## Types
 Swift includes various types that can be used in different ways in a program or app. Here are some examples

| Type | Explanation | Examples |
|---|---|---|
|Int|An integer.  Can be positive, negative or zero.| 3, 0 -9|
|Double|A number with a decimal| 3.2934, -39.99, 3.00|
|Character|A single character| "d", "!"|
|String|Zero or more characters chained together|"Hi my name is Iram", "", "What's your name? "|
|Bool|A truth value that can either be true or false |true, false|

## Variables and Constants 
**Variable** - piece of information that is stored with two components, a name and a value. The value can be accessed and changed later.
**Constant** - just like a variable it stores a value via a name. However, the value stored cannot be changed once it is declared.

A variable can be thought of as a box that has a label and contents inside. The label is the name of the variable and the contents is the value it stores. Lets see some examples.

```swift
let myName = "Iram" // constant
var myAge = 24 // variable
var metrocardFare = 2.75 //variable
```

## Conditionals and Control Flow 
Now that we can make variables, we can write very simple programs that maipulate these variables. Conditionals allows us to write code that can do different things depending on if certain conditions are met. This is called Control Flow. 

## if/else 

### if
an if block is very common in swift and is a basic example of conditionals and control flow. 

```swift 
if //conditional expression 
{
//block of code to be executed 
}
```
the `if` keyword allows us to test a set of conditions. If the expression after the `if` equates to true then the code in the curly braces {} will be executed. 

```swift 
var temperatureInFahrenheit = 30
if temperatureInFahrenheit <= 32 {
    print("It's very cold. Consider wearing a scarf.")
}
```
What would we expect to happen after the code above is run? 

### else 
were the `if` condition be false, we can set code inside an `else` block to be run 

```swift 
temperatureInFahrenheit = 40
if temperatureInFahrenheit <= 32 {
    print("It's very cold. Consider wearing a scarf.")
} else {
    print("It's not that cold. Wear a t-shirt.")
}
```

### else if 
We can also include `else if` in case we want to check multiple conditions.

```swift 
temperatureInFahrenheit = 90
if temperatureInFahrenheit <= 32 {
    print("It's very cold. Consider wearing a scarf.")
} else if temperatureInFahrenheit >= 86 {
    print("It's really warm. Don't forget to wear sunscreen.")
} else {
    print("It's not that cold. Wear a t-shirt.")
}
```
## Functions 
Functions are a fundmental part of swift. In short, a function is a piece of code that we can store and use at any time. A function may have input, and also may have output.

```swift 
func helloWorld() {
print("Hello World")
}
```
The code above is a very simple function. Whenever it is called, it simply prints "Hello World"
```swift 
helloWorld()
```
Lets take a look at a more dynamic example 

```swift
func doubleANumber(number x: Int) -> Int {
	let doubledNumber = 2 * x
	return doubledNumber
}
```
In the example above our function takes an Int. This Int has an external paramater name of number and internal paramter name of x. So when we call the function we see number, but if we want to access the Int in the body of the function we use x. In this function we also specify that we will return a value of type Int. 

lets try it out 
```swift
doubleANumber(number: 5)
```

