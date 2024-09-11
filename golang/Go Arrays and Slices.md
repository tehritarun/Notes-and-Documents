#### Defining array
An array can be defined, similar to any other variable, with `var` keyword. An example for array definition is as below.
```go
var array [4]float64
array = [4]float64{4.0, 2.99, 3.99, 6.99}
fmt.Println(array)
```

We can also define and initialise it with concise notation
```
// concise notation here
```
#### Working with Arrays
```go
fmt.Println(array[2])
```

#### Creating Slices
```go
filteredArray := array[1:3]
fmt.Println(filteredArray)
fmt.Println(len(filteredArray))
fmt.Println(cap(filteredArray))
```

#### Dynamic Arrays or lists
```

```


[[Go Language]]
