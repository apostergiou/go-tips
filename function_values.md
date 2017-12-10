# Function values

Functions can be used as values.
For example we can pass them as function arguments or use them as return values.

```go
foo := func(x, y float64) float64 {
        // function used as return value
        return math.Sqrt(x*x + y*y)
}

// function used as function argument
fmt.Println(foo(3, 4))
```
