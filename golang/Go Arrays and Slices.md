#### Defining array
An array can be defined, similar to any other variable, with `var` keyword. An example for array definition is as below.
```go
var array [4]float64
array = [4]float64{1.99, 2.98, 9, 29}
fmt.Println(array)
```

Alternatively
```go
var array [4]float64 = [4]float64{1.99, 2.98, 9, 29}
fmt.Println(array)
```

We can also define and initialise it with concise notation
```go
array := [4]float64{1.99, 2.98, 9, 29}
fmt.Println(array)
```
#### Working with Arrays
Individual elements can be access by using `[]`. example is as below
```go
fmt.Println(array[2])
array[2] = 8.49

```

#### Creating Slices
A slice in go is just pointer to subsegment of an array. it's element can be accessed similar to arrays.
```go
filteredArray := array[1:3]
fmt.Println(filteredArray)
```
Further slices can be resliced and even can be expended beyond its current size. But these can be expended only to its right side. Maximum expansion of slice can be determined by `cap` function. while `len` function denotes it current size.
```go
fmt.Println(len(filteredArray))
fmt.Println(cap(filteredArray))
filteredArray = filteredArray[:3]
fmt.Println(filteredArray)
```
#### Dynamic Arrays or lists
List are array with dynamic length. A list can be defines and assign as below. Basically a list is slice to an array created by go in background.
```go
var list []float64 = []float64{1.99, 3.49, 7.29}
fmt.Println(list)

```

#### Maps
```
\\classical defination
```
concise defination
```
age := make(map[string]int)
```

#### Working with Maps
```
age["John"] = 30
age["Doe"] = 35
fmt.Println(age["Doe"])
```

#### Make Function
`make` function is a standard function that can be used to create empty arrays, list or other objects as well. some examples of make function.
```
array := make([4]float)
list := make([]float, 4)
list := make([]float, 4, 9)
go_map := make(map[string]int)
```

[[Go Language]]
