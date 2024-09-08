#### Throwing Errors
Error can be passed from a function using out parameter named `err` of `error` type. Example is as below.
```go
func getUserInput(prompt string) (string, error) {
	var inputVal string
	fmt.Print(prompt)
	fmt.Scan(&inputVal)
	if inputVal == "" {
		return "", errors.New("Invalid inout")
	}
	return inputVal, nil
}
```

#### Catching Errors
Standard function with possibility of exception during processing also provides output with same name. further these errors can either be neglected as shown below.
```go
value, _ := getUserInput("Enter Value: ")
```

Or, can be taken action as required. simple example is given below.
```go
value, err := getUserInput("Enter Value: ")
if err != nil {
    fmt.Println(err)
    return
}
```

go back to main page [[Go Language]]
