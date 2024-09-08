A struct is defined with keyword `struct`.  An example of a struct is provided below.
```go
package user

import "fmt"

type User struct {
	firstName string
	lastName  string
	email     string
}

func New(firstname, lastname, email string) User {
	return User{
		firstName: firstname,
		lastName:  lastname,
		email:     email,
	}
}

func (u User) OutputUser() {
	fmt.Printf("Firstname: %v\nLastname: %v\nEmail: %v\n", u.firstName, u.lastName, u.email)
}

func (u *User) ClearName() {
	u.firstName = ""
	u.lastName = ""
}
```



go back to main page [[Go Language]]