#### Running a file
you can run a file directly by using below command
``` shell
go run <file_path>
```

Further if `go.mod` is defined we can use below command also to run main package.
```shell
go run .
```

#### Building Package
- First we need to define `go.mod` by using following commands
```shell
go mod init example.com/<package_name>
```

- Then package can be built using following command
```shell
go build
```

go back to main page [[Go Language]]