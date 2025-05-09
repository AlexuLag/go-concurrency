# Sleeping Barber Problem

This program implements a solution to the classic Sleeping Barber problem using Go's concurrency features.

## Description

The Sleeping Barber problem is a classic inter-process communication and synchronization problem between multiple operating system processes. In this implementation:

- A barbershop has multiple barbers (Pablo, Juan, and Pedro)
- Clients arrive randomly at the shop
- Barbers sleep when there are no clients
- The shop has a limited waiting room capacity
- The shop operates for a fixed time period

## Features

- Concurrent implementation using Go goroutines
- Channel-based communication
- Non-blocking client handling
- Graceful shutdown mechanism
- Color-coded console output
- Configurable parameters:
  - Shop capacity
  - Number of barbers
  - Haircut duration
  - Operating hours
  - Client arrival rate

## Program Structure

- **BarberShop**: Main structure managing the shop's state
- **Channels**:
  - `ClientsChan`: Queue for waiting clients
  - `BarbersDoneChan`: Synchronization for barber completion
  - `shopClosing` and `closed`: Shop closure control
- **Barber Management**:
  - Each barber runs in its own goroutine
  - Barbers sleep when idle
  - Barbers wake up when clients arrive

## Implementation Details

- Uses Go channels for communication
- Implements non-blocking client queue
- Handles shop closure gracefully
- Tracks barber states (sleeping/awake)
- Manages waiting room capacity

## Execution

To run the program:

```bash
go run main.go
```

## Output

The program will show:
1. Shop opening message
2. Real-time client arrivals
3. Barber activities (sleeping, waking, cutting hair)
4. Client handling (seated or rejected)
5. Shop closure and statistics

## Dependencies

- `github.com/fatih/color` for colored console output

## Learning Points

This implementation demonstrates:
- Channel-based communication
- Goroutine management
- Non-blocking operations
- Graceful shutdown
- Concurrent state management 