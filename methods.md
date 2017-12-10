# Methods

In Go the `method` terminology is similar to that of OOP languages.
A function which takes a `receiver` is considered a method.

```go
// Usage:
// fooFunction(1)
func fooFunction(x int) {
        fmt.Println(x)
}

// Usage:
// a := theReceiver(1) or var a theReceiver = 1
// a.fooMethod(1)
type theReceiver int
func (a theReceiver) fooMethod (x int) {
        fmt.Println(x)
}
```
