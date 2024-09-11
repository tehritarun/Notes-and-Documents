### Program structure

``` go
package main

import "fmt"

func main(){
    // some code here
}
```

#### Example Hello world program

``` go
package main

import "fmt"

func main(){
    fmt.Println("Hello! world")
}
```

### Variables

a variable declaration start from keyword `var` as seen in example below.
while initiation is done with `=` operator.
``` go
var name string
```
although both declaration and initiation can be done in single line. in multiple ways
``` go
var age int = 32 // this is standard type
var age = 32 // here type is inferred from value. int in this case.
var age = 32.0 // here .0 is added to value to force go to inferred this value as float
age := 32.0 // this is same as line 3 in compact notation
```

### Conditional statements
#### if statement
``` go
if age >= 30 {
    fmt.Println("Adult")
}
```
#### else if statement
``` go
if age >= 30 {
    fmt.Println("Adult")
} else if age >= 21 {
    fmt.Println("non juvenile")
}
```
#### else statement
``` go
if age >= 30 {
	fmt.Println("Adult")
} else if age >= 21 {
	fmt.Println("non juvenile")
} else {
	fmt.Println("juvenile")
}
```
#### switch statement
``` go
var choice int
fmt.Scan(choice)
switch choice {
case 1:
    fmt.Println("option 1 is chosen")
case 2:
    fmt.Println("option 2 is chosen")
case 3:
    fmt.Println("option 3 is chosen")
default:
    fmt.Println("invalid option is chosen")
}
```
### Loops
#### Conditional loop
``` go
for <condition> {
    // repeating code here
}
```
#### Infinite loop
``` go
for {
    // infinitly repeating code here
}
```
#### Standard for loop
``` go
for i:=0;i<10;i++ {
    // repeating code here
}
```

#### Loop for arrays and list
```
// loops for arrays and list
```
go back to main page [[Go Language]]
