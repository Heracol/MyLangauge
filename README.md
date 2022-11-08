# The Pra Language

## Introduction
Pra Language is an easy to learn programming language. It has efficient data structures. Pra Language has simple and elegant syntax and dynamic typing. It's interpreted nature, makes it an ideal language for scripting programs for windows.

## Basics of Pra Language

### Starting the program
To start the interpreter you can just open the executable. Pra Lanugauge programs end with ".pra". To run a seperate file you can pass the files path as the first argument to the program.

### Numbers in Pra Language
The syntak is simple: +, -, \*, /. It also has the power operator ^ e.g. x ^ y, which is the same as x<sup>y</sup>. You can also use parentheses to give it a higher priority. The modolo operator % returns the remainder of the division.
```
>>> 5 + 3
8
>>> 3 + 2 * 4
11
>>> (3 + 2) * 4
20
>>> 5 / 3
1.66667
```

### Conditions
A condition is either true or false. In Pra Language true equals 1 and false equals 0. A condition can be obtained by comparing two or more conditions. Comparing is done with ==, !=, <, >, <=, >=.

### Variables
Pra Language is a weakly typed language. It does not have any types. Variables names can be only be started with letters and \_. They cannot start with digits or any special charachters. Variables can overwrite existing values. Fuction names are also treated as variables. To define a variable use the = operator. The RHS is assigned to LHS. Variables can hold any value. The type of value can be changed any time.
```
>>> number = 6
>>> 6
>>> number = number + 5
>>> 11
```

### Strings
Strings are an important part of Pra Language. Strings are specified with "". Anything starting and ending with " is a string. String can hold any charachter. To append two strings use the + operator. Multiplying a string with a number returns a the string repeated n times. Using the indexer [] use can access each charachter.
```
>>> "hi " * 3 + "pra"
>>> "hi hi hi pra"
```

### Lists
Lists can store many values. To create a list use \[\]. This will return a empty list. To append a item to the list you can use the + operator. But list can be only appended by a list itself. To access a element of the list by index use the indexer operator \[i\]. Like strings lists can also be multipied with numbers. To get the length of a list use the len function.
```
>>> list = [1]
>>> [1]
>>> list = list + [2, 3]
>>> [1, 2, 3]
```

## If and Loops

### If Statement
The if statement checks if the condition is true and if is then executes the following code. You can have zero or more elif and an optional else. The code to run is within the { ... }. In Pra Language if can also be an expression. For an expression you need if and else and need to be written in a single line without {}. For a single line if statement you can avoid {} and write on a new line.
```
if false
  ...
elif false {
  ...
  ...
}

val = 10 if true else 11
```

### While Loop
The while loop runs the code until the condition is false. Like the if statement while can also be written in a single line.
```
while (...) {
  ...
  ...
}
```

### For Loop
The for loop runs the code a specific number of times. A variable is declared with its starting value. Each iteration it add the step value to it. By default step is 1. The code runs until the value equals end value. Step is optional.
```
for i = 1 to 10 step 2
  ...
```

### break, continue, return

#### break
Break is used in loops. It will instantly jump out of the loop.

#### continue
Continue is used in loops. It will go to the next iteration without runing the code after it.

#### return
Return is used in function. It will jump out of the function and return the value.

## Functions

### In-Built Functions
In Pra Language there are some in-built functions. Some important of them are:

#### print(value)
The print function will print the given value to the console. Value can be anything.

#### input(string)
The input function will wait for the user to input something. It will wait for the user to press enter. It will return a string.

#### clear()
Clear will clear the console and place the cursor to the top left.

#### require(filename)
This function will run the given file.

#### len(list)
It return the lenth of the list or string.

#### num(string)
Num converts the given string to number.

### Calling Functions
To call a function use (). Parameters can be passed through the parentheses.
```
>>> print("hello world")
>>> hello world
```

### Defining Functions
To define a function use this format:
```
func name : var_a, var_b {
  ...
  ...
}
```
When no parameters are needed, : is not needed. To define this function in a single line use -> instead of {}. Like this:
```
func name : var_a -> ...
```
The function name is also optional. Without name you can't call the function unless you assign it to something.
```
myvar = func -> ...
```
A function can return a value or perform some operations. You can also assign functions to variables.
