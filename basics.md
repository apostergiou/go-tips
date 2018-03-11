// A variable can contain functions.
```go
func main() {
    action := func() {
	    // actions
	}
	action()
}
```


// constants are declared like variables but with the const keyword.

// The bin folder contains Go compiled libraries (executables).
// The pkg folder contains the compiled versions of the available libraries.
// The src folder contains the Go source code organized by import path.

// Exported names begin with a capitalized letter.

// Functions are always typed.

// By default Go passes arguments by value (copied arguments).
// Pointers can be used to pass arguments by reference.
// A structure with reference values like slices or map is passed by reference.

// Use T(v) to convert the value v to the type T.

// A type assertion provides access to an interface value's underlying
// concrete value.

// Structs support composition (embedding) but not inheritance.

// Go supports implicit composition.
```go
type Job struct {
    Name string
    *log.Logger
}

func main() {
	job := &Job{"foo", log.New(os.Stderr, "Job: ", log.Ldate)}
	job.Print("Starting...")
}
```

// An interface type is defined by a set of methods. A value of interface type
// can hold any value that implements those methods.






