# Dining Philosophers Problem

This program implements a solution to the classic dining philosophers problem using Go and concurrency.

## Description

The dining philosophers problem is a classic synchronization problem that illustrates the challenges of avoiding deadlock in a concurrent system. In this program:

- 5 philosophers (Plato, Socrates, Aristotle, Pascal, and Locke) are seated around a circular table
- Each philosopher needs two forks to eat
- Philosophers alternate between eating and thinking
- The program simulates this scenario using goroutines and mutexes to handle concurrency

## Features

- Concurrent implementation using Go goroutines
- Synchronization using mutexes for the forks
- Control of philosophers' completion order
- Configurable timings for:
  - Eating (2 seconds)
  - Thinking (3 seconds)
  - Wait time between actions (1 second)

## Program Structure

- Each philosopher is represented by a structure with a name and references to their forks
- Forks are implemented as mutexes
- WaitGroup is used to synchronize the start and end of the simulation
- The order in which philosophers finish eating is recorded and displayed at the end

## Execution

To run the program:

```bash
go run main.go
```

## Output

The program will show:
1. A welcome message
2. The simulation of philosophers eating and thinking
3. The order in which philosophers finish eating 