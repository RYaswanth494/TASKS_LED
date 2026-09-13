# RTOS Complete Syllabus

## 1. Fundamentals of Operating Systems
- What is an OS (General purpose vs Embedded vs RTOS)
- Types of RTOS (Hard, Firm, Soft real-time)
- Kernel structure (Monolithic, Microkernel, Nanokernel)
- Foreground/Background systems vs RTOS
- Polling vs Interrupt-driven systems

## 2. RTOS Basic Concepts
- Tasks/Threads
- Task States (Ready, Running, Blocked, Suspended, Terminated)
- Task Control Block (TCB)
- Context Switching
- Dispatcher
- Idle Task
- System Tick / Tick Timer

## 3. Scheduling
- Scheduling basics (Preemptive vs Non-preemptive)
- Scheduling Algorithms
  - Round Robin
  - FCFS
  - Priority-based Scheduling
  - Rate Monotonic Scheduling (RMS)
  - Earliest Deadline First (EDF)
  - Least Laxity First (LLF)
- Time slicing
- Multilevel Queue Scheduling
- Scheduling Latency & Jitter

## 4. Task Management
- Task Creation & Deletion
- Task Priorities
- Priority Assignment techniques
- Task Suspend/Resume
- Task Delay/Sleep functions
- Idle Hook / Tick Hook

## 5. Intertask Communication
- Message Queues
- Mailboxes
- Pipes
- Shared Memory
- Signals

## 6. Synchronization
- Semaphores
  - Binary Semaphore
  - Counting Semaphore
- Mutex
- Mutex vs Semaphore
- Critical Section
- Spinlocks
- Condition Variables
- Event Flags/Event Groups

## 7. Problems in RTOS & Solutions
- Race Condition
- Deadlock
  - Deadlock Prevention
  - Deadlock Avoidance
  - Deadlock Detection
- Livelock
- Starvation
- Priority Inversion
  - Priority Inheritance Protocol
  - Priority Ceiling Protocol

## 8. Memory Management in RTOS
- Static vs Dynamic Memory Allocation
- Memory Pools
- Stack Management per Task
- Stack Overflow Detection
- Heap Management (TLSF, First-fit, Best-fit)
- MPU (Memory Protection Unit) basics

## 9. Interrupt Handling
- ISR (Interrupt Service Routine) basics
- ISR vs Task
- Nested Interrupts
- Interrupt Latency
- Deferred Interrupt Processing (Bottom Half/Tasklets)
- Interrupt Priority Levels

## 10. Timers
- Hardware Timers vs Software Timers
- One-shot Timer
- Periodic Timer
- Timer Callback functions
- Watchdog Timer

## 11. RTOS Kernel Services (API level)
- Task APIs (create, delete, suspend, resume)
- Queue APIs
- Semaphore/Mutex APIs
- Timer APIs
- Event APIs

## 12. Popular RTOS (Practical exposure)
- FreeRTOS
  - Architecture
  - Configuration (FreeRTOSConfig.h)
  - Task creation example
  - Queue/Semaphore example
- Zephyr RTOS
- ThreadX (Azure RTOS)
- VxWorks
- RT-Linux / PREEMPT_RT patch
- μC/OS-II / μC/OS-III

## 13. Real-Time System Design
- Task Design Principles
- Worst Case Execution Time (WCET)
- Response Time Analysis
- Real-Time Constraints (Deadlines, Periods)
- Rate Monotonic Analysis (RMA)
- CPU Utilization Bound

## 14. Communication with Hardware
- GPIO handling in RTOS
- UART/SPI/I2C driver integration with RTOS
- DMA with RTOS
- Device Driver structure in RTOS

## 15. Power Management
- Tickless Idle Mode
- Low Power States
- Dynamic Voltage & Frequency Scaling (DVFS) awareness

## 16. Debugging & Analysis Tools
- RTOS-aware Debuggers
- Trace Tools (SEGGER SystemView, Percepio Tracealyzer)
- Stack usage analysis
- CPU load analysis
- Deadlock/Livelock detection tools

## 17. Advanced Topics
- Multicore RTOS / SMP (Symmetric Multiprocessing)
- AMP (Asymmetric Multiprocessing)
- Hypervisor + RTOS combination
- Mixed Criticality Systems
- Safety Standards (ISO 26262, DO-178C, IEC 61508)
- Formal Verification of RTOS
- Security in RTOS (Secure boot, TrustZone with RTOS)

## 18. RTOS Porting & Board Bring-up
- Porting RTOS to new hardware/microcontroller
- Board Support Package (BSP)
- Linker script for RTOS
- Bootloader interaction with RTOS

## 19. Project-based Learning (Practical)
- Blinking LED task with FreeRTOS
- Multiple task communication using Queue
- Producer-Consumer problem
- Priority Inversion demo
- Sensor data acquisition system (task + ISR + queue)
- Mini Real-Time project (e.g., traffic light controller, motor control)
