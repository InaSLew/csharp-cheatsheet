# CSharp Cheat Sheet Template

Keyword |                  Summary                   | Sample Code | Mentioned In
------- | ------------------------------------------ | ------------ | ------------
`;`     | Used to separate statements from each other.| `int i = 5; i++; Console.WriteLine(i);` | [Script Execution](https://github.com/marczaku/csharp-basics/blob/main/slides/003.3.1-console-basics-1.md#0-script-execution)
`//`    | Used for single-line comments              | `float multiplier = 0.01f; // % to float (e.g. 24% = 0.24)` | [Comments](https://github.com/marczaku/csharp-basics/blob/main/slides/003.3.1-console-basics-1.md#single-line-comments)
Variable Initialization | When a value is assigned to a variable for the first time | `int a = 5;` | [Variables](https://github.com/marczaku/csharp-basics/blob/main/slides/003.3.1-console-basics-1.md#variable-initialization)
`dotnet new console -o project-name` | CLI to create dotnet console project | `dotnet new console -o Battleships`  | ?
Script Execution Order | Execution of code is top-down and left-to-right | `` | ?
Formatting | the style in which the code is written, e.g. trailing open curly brace or break a new line for open curly brace | ? | ?
`Console.WriteLine` | The method prints out the given argument(s) into the terminal and break into a new line | `Console.WriteLine("Hello world") // will print "Hello world\n"` | ?
`Console.Write` | The method prints out the given argument(s) into the terminal **WITHOUT** any line-break | `Console.Write("Hello world") // will pint "Hello world"` | ?
Multi-Line Comment | Allow multi-line comments | `/*This is a multiline\n comment*/` | ?
XML Documentation Comment | Comments that can used to produce API documentation | `/// <summary>This class does...</summary>` | ?
Variable | a piece of memory to retain data for reference and/or manipulation by a computer program | ? | ?
Variable Declaration | Declare a variable of a data type but not assigning a value to it | `string greeting;` | ?
Variable Assignment | Assign a value to a variable | `greeting = "Morning!"` | ?
Uninitialized Variable | A declared variable  | ? | ?
`=` (Assignment Operator) | Assign value on the right-hand side to the left-hand side | `int a = 0 // assigning value 0 to int a` | ?
Scope | Wrapped within `{}` and dictates whether or not variables and methods are defined and available for operation | `for (int a = 0; a < 2; a++ { (...) }) // attempts to use variable a outside the for loop will throw a compiling error` | ?
Variable Scope | The scope in which a variable is defined | `for (int a = 0; a < 2; a++ { (...) }) // variable a's scope lies with the for-loop` | ?
`int` | a build-in value type that holds an integer | `int myInt = 0;` | ?
`float` | a floating point type that holds a number with decimal point, 4 bytes | `float myFloat = 0.5f` | ?
`double` | a floating point type that holds a number with decimal point, 8 bytes | `double myDouble = 0.5` | ?
`bool` | a boolean value type that holds either True or False | `bool isGameOver = false` | ?
`char` | holds one single Unicode character, wrapper between single quotes `''` | `char firstLetterInMyName = 'I';` | ?
`string` | holds a sequence of `char`s, wrapped between double-quotes `""` | `string myName = "Ina";` | ?
`byte` | Unsigned 8-bit integer, 0-255 | `byte max = 255;` | ?
Implicit Casting | Cast from one data type to another without any special syntax (no info lost) | `int a = 10; [...] float b = a; // no special syntax required` | ?
Explicit Casting | Cast from one data type to another using a cast expression due to potential information loss | `float a = 10f; [...] int b = (int)a; // Compiler requires explicit cast expression` | ?
Type Conversion | Converting from one data to another using the `Convert` class  | `int a = Convert.ToInt32("1");` | ?
`Convert.ToInt32` | Converts a specified value to a 32-bit signed integer. | `int a = Convert.ToInt32("1");` | ?
Operators | a character/characters that determine what action to take | ? | ?
Arithmetic Operators | Operators used to perform simple math operations | `int a = 4; int b = 2; a+b; a-b; a*b; a/b; a*b; a%b`; | ?
`+` | Plus the left-hand side to right-hand side; also does concatenation if expressions on both sides are `string`s | `int a = 0; int b = 1; int c = a + b; // expect 1 + 0 = 0` and `string helloWorld = "Hello " + "World"; // "Hello World"` | ?
`-` | Subtract the amount of right-hand side from the left-hand side | `int a = 4; int b = 2; int c = a - b; // expect c == 2` | ?
`*` | Multiply the left-hand side value with the right-hand side | `int a = 2; int b = 0; int c = a * b; // expect c == 0` | ?
`/` | Divide the left-hand side with the right-hand side | `int a = 4; int b = 2; int c = a / b; // expect c == 2` | ?
`%` | Returns the remainder of dividing the left-hand side with the right-hand side | `int a = 10; int b = 2; int c = a % b; // expect c == 0` | ?
`+=` | Plus the right-hand side value to left-hand side and re-assign the new value to left-hand side | `int a = 0; a += 1; //expect a == 1` | ?
`-=` | Subtract the right-hand side value from left-hand side and re-assign the new value to left-hand side | `int a = 0; a -= 1; //expect a == -1` | ?
`++` | Increment by 1 | `int a = 0; a++; // expect a == 1` | ?
`--` | decrement by 1 | `int a = 0; a--; // expect a == -1` | ?
Post-Increment `i++` | evaluate the expression **THEN** increment | ? | ?
Pre-Increment `++i` | increment **FIRST THEN** evaluate the expression | ? | ?
`System.Math` | A library provided by c# for common math operations | `using System.Math;` | ?
`static` | a modifier used to indicate that a class or its member(s) belongs to the type rather than an instance, i.e. can only be used on `Type` | `static void Main() {...} // Program.Main();` | ?
`Math.Max` | a method that returns the larger of two given numbers | `Math.Max(0, 100); // expect to return 100` | ?
`Math.Min` | returns the smaller of two given numebrs | `Math.Min(0, 100); // expect to return 0` | ?
`Math.Sqrt` | returns the square root of the given number | `Math.Sqrt(4); // expect to return 2` | ?
`Math.Abs` | returns the absolute value of the given number | `Math.Abs(-100); // expect to return 100` | ?
`Math.Round` | returns value to the nearest integer or to the specified number of fractional digits | `float a = 0.95; double b = Math.Round(a); // expect a == 1` | ?
`Math.Floor` | returns the largest integral value less than or equal to the specified number. | `float a = 0.95; double b = Math.Floor(a); // expect a == 0` | ?
`Math.Ceiling` | returns the smallest integral value greater than or equal to the specified number. | `float a = 0.95; double b = Math.Ceiling(a); // expect a == 1` | ?
`Math.Clamp` | takes 3 arguments `value`, `min` and `max`, returns a value clamped to the inclusive range of `min` and `max` | `Math.Clamp(2000, 0, 100); // expect to return 100;` | ?
`Math.Pow` | returns a specified number raised to the specified power. | `Math.Pow(2, 0); // 2 to the power of 0, expect to reutrn 0` | ?
`string.Length` | returns the length of the `string` | `"Cat".Length; // expect to be 3` | ?
`string.ToUpper` | returns a copy of the `string` converted into uppercase. | `"cat".ToUpper(); // expect to be "CAT"` | ?
`string.+` | string concatenation | `"Hello " + "World" // expect to be "Hello World"` | ?
`$"{}"` | string interpolation, able to evaluate expressions | `$"1 + 1 = {1+1}" // expect "1 + 1 = 2"` | ?
`string.[]` | access the `string` as an array of `Char` with the index | `"Hello"[0]; // expect to be 'H'` | ?
`string.IndexOf` | returns the index of the first slot in the array that matches the given value | `"Hello".IndexOf("l"); // expect to be 2` | ?
`string.SubString(int)` | returns a substring of the instance starting from `string[int]` | `"Hello".Substring[1]; // expect to be "ello"` | ?
`string.Substring(int, int)` | returns a substring of the instance starting from `string[int]` and up to `string[int]` | `"Hello".Substring[1, 3]; // expect to be "ell"` | ?
`string.Replace` | returns a new string in which all occurrences of a specified `char` or `string` in the current string are replaced with another specified Unicode character or String | `"Hello".Replace("ello", "i"); // expect to be "Hi"` | ?
immutable | State cannot be modified after created | `string t = "TEst"; t[1] = "e"; // compiler error becasue string is immutable` | ?
Logical Operators | symbols to connect two or more expressions and evalute to true or false | `&&`, `||`,`!` | ?
`!` | negates the following expression | `0 != 1` | ?
`&&` | both left- and right-hand sides need to be true to evaluate to true | `true && false; // expect to return false` | ?
`||` | if left-hand side is true then returns true; othersise evalute right-hand side returns its value | `false || true; // expect to return true` | ?
Comparison Operators | comparing the left- and right-hand side values and returns true or false | ? | ?
`>` | left-hand side is greater than right-hand side | `2 > 1; // expect to be true` | ?
`==` | left-hand equals to right-hand side | `1 == 0; // expect to be false` | ?
`!=` | left-hand does not equal to right-hand side | `1 != 0; // expect to be true` | ?
`>=` | left-hand side is greater than or equal to right-hand side | `1 >= 1; // expect to return true` | ?
`<=` | left-hand side is smaller than or equal to right-hand side | `1 <= 1; // expect to return true` | ?
`if` | if the given expression evaluates to true then execute the if-clause | `if (true) { Console.WriteLine("True"); } else { Console.WriteLine("False"); } // expect "True"` | ?
`else` | if the given expression evaluates to false then execute the else-clause | `if (false) { Console.WriteLine("True"); } else { Console.WriteLine("False"); } // expect "True"` | ?
`else if` | if `if` is followed by one or more `else if`, check them from top-to-down and executes the first `else if` that evaluates to true | ? | ?
`? :` | ternary operator, if the expression on the left-hand side of `?` evaluates to true then executes the left-hand side of `:`, if false then the right-hand-side of `:` | `Console.WriteLine(true ? "True" : "False"); // expect "True"` | ?
Flow Control Statements | statements to control the flow of execution | ? | ?
`System.Random` | The random class available in the System library, used for generating random numbers | `Random random = new Random();` | ?
pseudo-random | The "random" number returned from using `Random` is not true, but a close imitation of it | ? | ?
seed | `Random` also takes a seed upon instantiation; same seed will result in the same set of random numbers | ? | ?
`Random.Next(int, int)` | returns a random number between the first and the second int(second int NOT included) | `var randomNumnber = new Random().Next(0, 3); // expect a number between 0 to 2, not including 3` | ?
`Random.Next()` | returns a non-negative random integer | `new Random().Next(); // literally any integer that an int type holds` | ?
`Random.NextDouble()` | returns a non-negative random double | `new Random().NextDouble(); // expect any number that a double type holds` | ?
`while` | a loop that will only end when the given predicate evaluates to false | `var a = 0; while (a < 2) { a++; } // loop will end when it got incremented to 2 and evaluates to false in the predicate` | ?
bool-expression | an expression that evaluates to a boolean | `1 == 5;` | ?
`do..while` | the `do`-clause will be executed once before entering the `while` loop | `var a = 0; do { a++ } while (a == 0); // while-loop will end right after it got incremented inside the do-clause and evaluates to false in the predicate` | ?
`for` | will execute while the statement in the for statement evaluates to true | `for (var i = 0; i < 2; i++) { Console.WriteLine(a); } // expect to print 1 and 2 in two lines` | ?
iteration statement | the statement that if evaluated to true will allow the loop to keep looping | `for (var i = 0; i < 2; i++) { Console.WriteLine(a); }` | ?
loop body | loop body gets executed every time the loop statement evaluates to true | `for (var i = 0; i < 2; i++) { Console.WriteLine(a); }` | ?
loop | one iteration of the loop body | ? | ?
execution | running of the program | ? | ?
execution jump | ? | ? | ?
`break` | break out of the current loop completely | ? | ?
`continue` | skip the rest of the loop body after `continue` and enter the next loop | ? | ?
`Array` | a collection of items of the same data type stored at contiguous memory locations | ? | ?
`int[]` | an array of type int | ? | ?
Array Initialization | declare an array and assign value to it | ? | ?
Array Access for Assignment | assign a value to a slot in an array through specified index number | `myArray[0] = 0;` | ?
Array Access for Reading | access a slot in an array through specified index number | `myArray[0]; // accessing the first slot in myArray` | ?
`Array.Resize` | change the number of elements of a one-dimension array to a specified size | ? | ?
`Array.Length` | returns the length of the array | `String[] myArr = {"The", "quick", "brown", "fox", "jumps", "over", "the", "lazy", "dog"}; var length = myArr.Length; // expect 9` | ?
`foreach` | enumerates the elements of a collection and executes its body for each element of the collection. | ? | ?
`2D-Array` | Multiple one-dimension arrays inside a one-dimension array | `[[],[],[],[],[],[],[],[],[]]` | ?
2D-Array Initialization | declare and assign value to a 2D array | `string[,] my2DArray = new string[3,3] { {"", "", ""},{"", "", ""},{"", "", ""} }` | ?
2D-Array Access for Assignment | accessing a slot in the 2D array through specified indexes | `my2DArray[1,1] = <3` | ?
2D-Array Access for Reading | assigning a value to a cell inside the 2D array through specified indexes | `Console.WriteLine(my2DArray[1,1]); // expect to print "<3"` | ?
Jagged Arrays | a multi-dimension array where the member arrays are of different length | ? | ?
Method | a function member of a class | ? | ?
`void` | a return type that means the function/method returns nothing | ? | ?
Return Type | a data type that a function/method promises to return | ? | ?
`()` | immediate invocation | `var canEat = false; Console.WriteLine($"Can you eat? {(canEat ? "YASSSS" : "Nope")}");` | ?
Parameter | in a function/method signature to specified the variables the said function/method requires as input | ? | ?
Argument | the input(s) given to a function/method invocation per the parameter list's specification | ? | ?
Parameter-List | specified in a method/funtion's signature to indicate what the said function/method needs for input | ? | ?
Named Arguments | specified which parameter this argument  | ? | ?
Optional Arguments | parameters that have default values make theirs arguments in invocation optional| ? | ?
Default Value | a default value that a function/method uses if none is given through the argument | ? | ?
`return` | return a value if any is given and then exit the function/method | ? | ?
Code Paths | the set of specific instructions that got executed during a single run of program/program fragment | ? | ?
Method Overloading | Methods of the same name but with different parameter lists | ? | ?
Object-Oriented Programming | a programming paradigm where code is encapsulated and abstracted into objects  | ? | ?
Data | the thing that a computer program manipulates | ? | ?
Function | (ideally) a set of code that performs a specific task indicated by its name | ? | ?
Structured Programming | a programming paradigm where a program is broken into smaller functions/modules | ? | ?
Objects | an instance of a class | ? | ?
Instance Method | methods that are available for invocation on an object instance | ? | ?
Class | model representation of something, data fields for the data this something has, and methods for what this something does  | ? | ?
Type | Specify common features of a set of class | ? | ?
`class` | keyword to use when declaring a class | ? | ?
`new` | keyword for when instantiating a new object instance of a class | ? | ?
Class Member | data fields and methods inside a class | ? | ?
Class Instance | an object | ? | ?
Garbage Collector | automatic memory management; in charge of allocating and freeing up memory for programs | ? | ?
`null` | a special data type that can only have one value (`null`) and signalfies that no value is assigned | ? | ?
Invoke | calling of a method/function | ? | ?
Field | holds data inside a class | ? | ?
Static Class Member | static data fields and methods inside a class | ? | ?
Static Class | a class that's entirely static | ? | ?
Global Access | when a function/method/variable is on a global scope, anywhere in the program has access to it | ? | ?
Constructor | a special method that is called upon instantiation to give the instance initial values | ? | ?
Initial Class Values | the inital values given through constructor? | ? | ?
Parameterless | When a method/function signature doesn't take any parameter | ? | ?
Default Contructor | an invisible default constructor that will return an empty instance, can be overriden | ? | ?
Finalizer | the method that's called upon destroying of an object | ? | ?
Object Destruction | object destroyed when not being used or stored in a variable | ? | ?
`GC.Collect` | Invoking `GC.Collect()` to force garbage collection | ? | ?
Encapsulation | encapsulating relevant functions and variables in one place, e.g. a class with data fields and methods | ? | ?
Access Modifier | modifies access right to a class and/or its members | ? | ?
`private` | accesssible only within the class | ? | ?
`protected` | accessible from within the class and derived classes | ? | ?
`public` | accessible through the same assembly(i.e. project) and other assemblies that reference it | ? | ?
`internal` | accessible through the same assembly | ? | ?
Class Member Access | Access modifier on the members of a class | ? | ?
Inheritance | deriving a class from a base class, where the derived class inherits the base class' protected members | ? | ?
Property | syntax sugar for getting and setting data fields in class | ? | ?
Getter Method | return the value of the property | ? | ?
Setter Method | set the value of the property | ? | ?
Validation | steps to check if sth is in the correct format for processing | ? | ?
Processing | (see above for Validation) | ? | ?
`get` | used to declare getter method for a property | ? | ?
`set` | used to declare setter method for a property | ? | ?
Expression Body Syntax | ? | ? | ?
Auto Property | When declared, the compiler creates private, anonymous backing fields that can only be accessed through the property's getter and setter | ? | ?
Read-Only Property | a property whose value assignment is only available upon declaration or inside the constructor | ? | ?
base-Class | the class a derived class is inheriting from | ? | ?
Inherit From | the action from which a derived class is created | `class Dog : Animal` | ?
Derived Class | the class that inherits from a base class | ? | ?
Child Class | another word for derived class | `class Cat: Animal {} // Cat is the child class` | ?
Parent Class | another word for base class | `class Cat: Animal {} // Animal is the parent class` | ?
`sealed` | to prevent a class from being inherited | ? | ?
Polymorphism | refers to that, despite of inheriting from the same base class and having its behaviors, the derived classes can look very different from the base class, as if the base class polymorphs  | ? | ?
`as` | to explicitly convert an expression to a given type | ? | ?
`virtual` | make a method/data field available for overriding in derived classes | ? | ?
`override` | derived class implements and overrides virtual methods/fields of the same name from the base class | ? | ?
`base` | used inside a derived class to reference the base class | ? | ?
Abstraction | the practice of hiding away the details of implementation and all the user needs to know is what input to give and what output to expect | ? | ?
`abstract` | make a class abstract, indicating it's for base class use only | ? | ?
Implementation | A system for executing computer programs? (compilation, e.g. C# vs interpretation e.g. javascript, python...etc) | ? | ?
Composition | class having properties that makes sense (e.g. a Hero class that has the property of type Weapon, instead of inheriting from the Weapon class) | ? | ?
"Composition over Inheritance" | Inheritance isn't always the right software design choice, in fact if possible, sensible composition goes first, then inheritance | ? | ?
