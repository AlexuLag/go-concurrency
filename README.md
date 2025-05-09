# Go Concurrency Examples

This repository contains three classic concurrency problems implemented in Go, demonstrating different aspects of concurrent programming.

## Projects

### 1. Dining Philosophers Problem
**Location**: `dinning-philosophers/`

A solution to the classic dining philosophers problem, where:
- 5 philosophers (Plato, Socrates, Aristotle, Pascal, and Locke) sit around a circular table
- Each philosopher needs two forks to eat
- Philosophers alternate between eating and thinking
- Implements deadlock prevention using mutexes

**Key Concepts**:
- Mutex synchronization
- Deadlock prevention
- Resource sharing
- Concurrent state management

### 2. Producer-Consumer Pattern
**Location**: `producer-consumer/`

A pizzeria simulation implementing the producer-consumer pattern:
- Producer creates pizza orders
- Consumer processes these orders
- Handles success and failure scenarios
- Tracks statistics and performance

**Key Concepts**:
- Channel-based communication
- Producer-Consumer pattern
- Error handling
- Concurrent processing

### 3. Sleeping Barber Problem
**Location**: `barber-shop/`

An implementation of the sleeping barber problem:
- Multiple barbers (Pablo, Juan, and Pedro)
- Random client arrivals
- Limited waiting room capacity
- Barbers sleep when idle

**Key Concepts**:
- Channel synchronization
- Non-blocking operations
- Graceful shutdown
- Resource management

## Common Features

All projects demonstrate:
- Go's concurrency primitives (goroutines, channels)
- Synchronization mechanisms
- Error handling
- State management
- Real-world problem solving

## Dependencies

- Go 1.x
- `github.com/fatih/color` for colored console output

## Running the Projects

Each project can be run independently:

```bash
# Dining Philosophers
cd dinning-philosophers
go run main.go

# Producer-Consumer
cd producer-consumer
go run main.go

# Sleeping Barber
cd barber-shop
go run main.go
```

## Learning Objectives

These projects serve as practical examples of:
1. Concurrent programming in Go
2. Common concurrency patterns
3. Problem-solving with concurrent systems
4. Synchronization techniques
5. Resource management
6. Error handling in concurrent systems

## Best Practices Demonstrated

- Proper use of goroutines
- Channel-based communication
- Mutex synchronization
- Graceful shutdown
- Error handling
- Resource cleanup
- State management
- Concurrent testing

