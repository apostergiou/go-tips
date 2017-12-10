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

## Buffered channels

Passing a second parameter to the make function creates a buffered channel:

```go
c := make(chan int, 1)
```

This creates a buffered channel with capacity of 1.
Channel communication is synchronous normally. Both sides of the channel wait
the other side to read or write a message.

Buffered channels are asynchronous. Sending or receiving a message is not a
blocking procedure unless the channel is full.

## References

- https://golang.org/ref/spec#Channel_types
