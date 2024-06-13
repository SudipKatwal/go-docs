# Go Basics

### Go's Basic Syntax

- let's start with "Hello world!" program

```
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

- Here's a brief explanation of each line:
  - **Package main**: This defines the package name for the current file. The main package is the entry point of Go applications.
  - **import "fmt"**: This imports the "fmt" package, which provides formatted I/O functions.
  - **func main() { ... }**: This declares the main function, which is executed when the program runs. The curly braces ({}) define the function body.
  - **fmt.Println("Hello, World!")**: This line calls the Println function from the "fmt" package to print "Hello, World!" followed by a newline.

### Go's Data Types

- Go has several built-in data types, including:

  - **Basic types**: bool, int, float64, complex128, string
  - **Aggregate types**: array, slice, struct
  - **Reference types**: pointer, channel, map, interface

- Example of defining the veriable with data types

  ```
  var b bool = true
  var i int = 2024
  var f float64 = 2024.06
  var c complex128 = 1 + 2i
  var s string = "Sudip Katwal"

  var arr [3]int = [3]int{1, 2, 3}
  var sl []int = []int{1, 2, 3}
  var st struct { x int; y int } = struct { x int; y int }{1, 2}

  var p *int = &i
  var ch chan int = make(chan int)
  var m map[string]int = make(map[string]int)
  var iface interface{} = "text"

  ```

- To declare a variable, use the var keyword followed by the variable name, its type, and an optional initializer

  ```
  var x int
  var y int = 10
  z:= 30 // shorthand syntax in Go for declaring and initializing variables
  ```

- We can also declare multiple variables in one line

  ```
  var a, b, c int = 1, 2, 3
  ```

- To declare a constant, use the const keyword:

  - A constant is a value that remains unchanged during the execution of a program. Once a constant is defined, its value cannot be modified or reassigned throughout the program's execution.

  ```
  const PI float64 = 3.14159265359

  ```

# Control Structures

> Control statems are the instructions that control the flow of program. It determines which code should be execute in certain condition or how many time code should be repeated. Some of the control statements in Go are:

- If else statement
- Switch statement
- For loop:
- blank identifier
- While loop
- Defer: Defer statement will be executed only after the surrounding function is executed.
  ```
  defer functionName(arguments)
  ```
- Break and Continue
- There is no do or while loop, only a slightly generalized for; switch is more flexible
