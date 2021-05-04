# RTOS



# FreeRTOS (C)

Real-time operating system for microcontrollers

Developed in partnership with the world’s leading chip companies over a 15-year period, and now downloaded every 170 seconds, FreeRTOS is a market-leading real-time operating system (RTOS) for microcontrollers and small microprocessors. Distributed freely under the MIT open source license, FreeRTOS includes a kernel and a growing set of IoT libraries suitable for use across all industry sectors. FreeRTOS is built with an emphasis on reliability and ease of use.


<https://www.freertos.org/>

<https://www.freertos.org/Documentation/RTOS_book.html>

AWS compatible.


# Mbed  

<https://os.mbed.com/mbed-os/>

RTOS core based on the widely used open-source CMSIS-RTOS RTX.


<https://os.mbed.com/docs/mbed-os/v6.10/introduction/index.html>

# Full Profile

The full profile of Mbed OS is an RTOS (it includes an RTX and all RTOS APIs), so it supports deterministic, multithreaded, real-time software execution. The RTOS primitives are always available, allowing drivers and applications to rely on threads, semaphores, mutexes and other RTOS features. It also includes all APIs by default, although you can remove unused ones at build time.

## Bare Metal Profile 

The bare metal profile doesn't include an RTX and is therefore not an RTOS - it is designed for applications that do not require complex thread management. It is also designed for constrained devices, and therefore focuses on minimising the size of the final application: by default, it includes only the smallest possible set of APIs, to which you can manually add APIs your application requires. The bare metal profile can use the small C libraries (which are not thread safe) to further minimise the size of the application. Mbed 2 users who want to move to Mbed OS 6 should use the bare metal profile.


## Licensing

We release Mbed OS under an Apache 2.0 license, so you can confidently use it in commercial and personal projects.



# Real-Time Interrupt-driven Concurrency (RTIC) framework (Rust)

A concurrency framework for building real-time systems.

Formerly known as Real-Time For the Masses.

<https://docs.rs/rtic-core/0.3.1/rtic_core/>

<https://rtic.rs/0.5/book/en/>

Embedded Rust

<https://docs.rust-embedded.org/book/intro/index.html>

Embedded Rust Details

<https://docs.rust-embedded.org/embedonomicon/>

# License

All source code (including code snippets) is licensed under either of

* [Apache License, Version 2.0 LICENSE-APACHE](https://www.apache.org/licenses/LICENSE-2.0)
* [MIT license LICENSE-MIT](https://opensource.org/licenses/MIT)

at your option.


# Tasks 

as the unit of concurrency [^1]. Tasks can be event triggered (fired in response to asynchronous stimuli) or spawned by the application on demand.

# Message passing

MP between tasks. Specifically, messages can be passed to software tasks at spawn time.

# A timer queue 

Software tasks can be scheduled to run at some time in the future. This feature can be used to implement periodic tasks.


# preemptive multitasking

Support for prioritization of tasks and, thus, preemptive multitasking.


# Efficient and data race free memory sharing
    
through fine grained priority based critical sections.

# Deadlock free execution

guaranteed at compile time. This is an stronger guarantee than what's provided by the standard Mutex abstraction.

# Minimal scheduling overhead.

The task scheduler has minimal software footprint; the hardware does the bulk of the scheduling.

# Highly efficient memory usage

All the tasks share a single call stack and there's no hard dependency on a dynamic memory allocator.

# All Cortex-M devices are fully supported.

# Worst Case Execution Time WCET

This task model is amenable to known WCET (Worst Case Execution Time) analysis and scheduling analysis techniques. (Though we haven't yet developed Rust friendly tooling for that.)


# Resumen

The future of rust RTOS' is much more promising than the future of C RTOS', there is so much room for innovation; take a look at r3 for example, which leverages unstable rust features. Unfortunately the reality is C RTOS' are much more mature.

<!-- https://docs.rs/r3/0.1.1/r3/ -->
