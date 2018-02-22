# iota

Go's iota identifier is used in const declarations to simplify definitions of
incrementing numbers.

## Example

```go
package main

import (
	"fmt"
)

const (
	x = (iota*2) + 1
	_ // blank identifier for ignoring a value
	y
	z
)

func main() {
	fmt.Println(x, y, z) // outputs: 1 5 7
}
```
