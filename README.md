# Go Race Condition Example

This repository demonstrates a potential race condition in a Go program involving channel operations.  The program uses two goroutines and a channel to illustrate a scenario where the channel is closed before all receivers have completed reading from it.

While this particular example might not always exhibit the race condition, it highlights a common pattern that can lead to unexpected behavior and data corruption in concurrent Go programs. The solution shows how to properly handle channel closure and prevent the race condition.

**How to Run:**

1. Clone this repository.
2. Run `go run bug.go` to observe the potential race condition. 
3. Run `go run bugSolution.go` to see the corrected version that avoids the race condition.