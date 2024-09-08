A struct is defined with keyword `struct`.  An example of a struct is provided below.
```go
package user

import "fmt"

type User struct {
	firstName string
	lastName  string
	email     string
}
```
#### Constructor
constructor is function that is used to instanciate struct. or used to create instance of struct
```go
func New(firstname, lastname, email string) User {
	return User{
		firstName: firstname,
		lastName:  lastname,
		email:     email,
	}
}
```

#### Methods
##### Simple method
Struct method is a function that processes instance of a struct. it usually defined similar to function only but '(<struct_name>)' before function name. Example method is shown as below.
```go
func (u User) OutputUser() {
	fmt.Printf("Firstname: %v\nLastname: %v\nEmail: %v\n", u.firstName, u.lastName, u.email)
}
```
##### Mutating method
A method that changes struct property can be called mutating method. Unlike simple method, we need to pass pointer to struct instead of struct itself. Note here that we can de-refrence the struct while updating its value. But that is optional and can be skipped for cleaner code as go handles that in background anyway.
an example of such method is provided below.
```go
func (u *User) ClearName() {
	u.firstName = ""
	u.lastName = ""
}
```



go back to main page [[Go Language]]
