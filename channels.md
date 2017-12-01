# About channels

> A channel provides a mechanism for concurrently executing functions to
communicate by sending and receiving values of a specified element type. The
value of an uninitialized channel is nil.

## Information direction

Arrows can indicate the information direction in regards to the channel
(input, output, input/output).

```go
chan <- // write to channel (output)
<- chan // read from channel (input)
chan    // (input/output)
```

## References

- https://golang.org/ref/spec#Channel_types
