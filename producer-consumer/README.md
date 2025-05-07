# Producer-Consumer Pattern: Pizzeria Simulation

This program demonstrates the producer-consumer pattern in Go through a fun pizzeria simulation. It shows how concurrent programming can be used to handle multiple tasks simultaneously in a real-world scenario.

## Description

The program simulates a pizzeria where:
- A producer (pizzeria) creates pizza orders
- A consumer processes these orders
- The system handles success and failure scenarios
- Results are tracked and displayed with color-coded output

## Features

- Concurrent implementation using Go channels
- Producer-Consumer pattern demonstration
- Error handling and graceful shutdown
- Color-coded console output for better visualization
- Random delays to simulate real-world processing time
- Success/failure tracking and statistics

## Program Structure

- **Producer**: Handles pizza order creation and channel management
- **PizzaOrder**: Structure containing order details and status
- **Channels**: 
  - `data` channel for pizza orders
  - `quit` channel for graceful shutdown
- **Statistics Tracking**:
  - Number of pizzas made
  - Number of failed orders
  - Total attempts

## Implementation Details

- Uses Go channels for communication between producer and consumer
- Implements graceful shutdown mechanism
- Random delays (1-5 seconds) to simulate pizza preparation time
- Random success/failure scenarios to demonstrate error handling
- Color-coded output using the `fatih/color` package

## Execution

To run the program:

```bash
go run main.go
```

## Output

The program will show:
1. Opening message
2. Real-time pizza order processing
3. Success/failure messages for each order
4. Daily statistics and performance summary
5. Color-coded performance rating

## Dependencies

- `github.com/fatih/color` for colored console output

## Learning Points

This implementation demonstrates:
- Channel-based communication in Go
- Producer-Consumer pattern implementation
- Concurrent programming concepts
- Error handling in concurrent systems
- Graceful shutdown of goroutines 