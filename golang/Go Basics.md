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
    fmt.println("Adult")
}
```
#### else if statement
``` go
if age >= 30 {
    fmt.println("Adult")
} else if age >= 21 {
    fmt.println("non juvenile")
}
```
#### else statement
``` go
if age >= 30 {
    fmt.println("Adult")
} else if age >= 21 {
    fmt.println("non juvenile")
} else {
    fmt.println("juvenile")
}
```
#### switch statement
``` go
switch choice {
    case 1:
    fmt.println("option 1 is chosen")
    case 2:
    fmt.println("option 2 is chosen")
    case 3:
    fmt.println("option 3 is chosen")
    default:
    fmt.println("invalid option is chosen")
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

go back to main page [[Go Language]]