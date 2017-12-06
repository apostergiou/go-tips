# Struct printing

Let's suppose we want to print a struct and some of its elements.
We can use the `%+v` verb. From the docs:

> %v the value in a default format when printing structs, the plus flag (%+v)
adds field names

```go
package main

import "fmt"

type cake struct {
	flavor    string
	price     int
	available bool
}

func main() {
	cake1 := cake{flavor: "chocolate", price: 10, available: true}
	cake2 := cake{flavor: "vanilla", price: 10, available: false}
	fmt.Printf("%s cake : %+v\n", cake1.flavor, cake1)
	fmt.Printf("%s cake: %+v\n", cake2.flavor, cake2)
}
```
