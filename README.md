# Unexpected Panic with Uninitialized Map in Go

This repository demonstrates a common error in Go: panics caused by accessing elements of an uninitialized map.  Uninitialized maps in Go are represented as `nil`, and attempting to access elements using the indexing operator (`map[key]`) on a `nil` map results in a runtime panic.

The `bug.go` file contains the buggy code, which panics when it tries to assign a value to a key in an uninitialized map. The `bugSolution.go` file provides a solution to prevent the panic using proper map initialization.