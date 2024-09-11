#### Importing Standard packages
Any package can be imported using keyword `import`. while standard package can be simply be imported using it's name as shown below.
```go
import "fmt"
```

while multiple packages can be imported with either multiple `import` statements or by using following notation.
```go
import (
	"errors"
	"fmt"
)
```
#### Creating custom package
In go every file starts with keyword `package` followed by package name it belongs to(Generally main).
note that a package can have multiple files associated with it. All files associated with a package should be contained in separate subfolder named same as package.
A package can be defined as below.
```go
package fileutil

import "os"

func Readfile(filename string) string {
	var value string
	fileBytes, _ := os.ReadFile(filename)
	value = string(fileBytes)
	return value
}

func WriteToFile(data string, filename string) {
	dataBytes := []byte(data)
	os.WriteFile(filename, dataBytes, 0644)
}
```

#### Importing custom package
A custom package can be imported in main package or other package as below
```go
import (
	"example.com/goapp/fileUtil"
)
```

Here, `example.com/goapp` is defined with `go mod` command here [[Go CLI#Building Package]].

#### Importing External Package
Before importing external package, it needs to be downloaded and added to the module. This process is described here [[Go CLI#Adding External Package]]. Then it can be imported into current package with `import` keyword as shown in example below.
```go
package main

import (
    "github.com/Pallinder/go-randomdata"
)
```

go back to main page [[Go Language]]