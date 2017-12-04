# Unused code and imports

Go refuses to compile programs with unused variables or imports.

To bypass this design decision (e.g. for bootstrapping or debugging sessions) we
can use:

```go
import "unused"

// This declaration marks the import as used by referencing an
// item from the package.
var _ = unused.Item  // TODO: Delete before committing!

func main() {
    debugData := debug.Profile()
    _ = debugData // Used only during debugging.
    ....
}
```

## References

https://golang.org/doc/faq#unused_variables_and_imports
