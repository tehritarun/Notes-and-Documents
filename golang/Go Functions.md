#### Simple Function
Function in go is defined by using keyword `func`. The example of a simple function is given below.
``` go
func sayHello() {
	fmt.Print("Hello!")
}
```

#### Input Parameters
``` go
func sayHello(name string) {
	fmt.Println("Hello!", name)
}
```

#### Output parameters
``` go
func getUserInput(prompt string) string {
	var inputVal string
	fmt.Print(prompt)
	fmt.Scan(&inputVal)
	return inputVal
}
```
The above function can also be written as below. Note here that out parameter is declared along with function. This we need not to mention it in return statement as well.
``` go
func getUserInput(prompt string) (inputVal string) {
	fmt.Print(prompt)
	fmt.Scan(&inputVal)
	return
}
```

go back to main page [[Go Language]]