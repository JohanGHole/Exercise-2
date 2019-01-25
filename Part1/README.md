# Mutex and Channel basics

### What is an atomic operation?
> Atomic operation is an operation that can not be interrupted. One cycle operation. 

### What is a semaphore?
> Variable used to control access to common resource by multiple processes in a concurrent system.

### What is a mutex?
> "Mutually exclusive flag" - controls which process that has access to a shared variable at a given time. 

### What is the difference between a mutex and a binary semaphore?
> mutex - only the thread that locked or unlocked the mutex can unlock it., like a token that is passed between the processes. Binary semaphore - 0/1. Traffic red light. Signals someone if they can proceed.

### What is a critical section?
> A critical section is a part of a program that accesses shared resources. Only when a process is in it's critical section can it be in a position to disrupt other processes (shared variables).  

### What is the difference between race conditions and data races?
 > Data race occurs when two instructions from different threads access the same memory location. At least one of these acceses is right, and there is no synchronisation. Race conditions is an error that occurs in the timing or ordering of events (Semantic error).

### List some advantages of using message passing over lock-based synchronization primitives.
> Message passing is useful for exchanging smaller amounts of data, because no conflicts need to be avoided. Better for safety concerns.

### List some advantages of using lock-based synchronization primitives over message passing.
> Shared memory is often faster than message passing. 
