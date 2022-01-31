## Operating System Assignments

---



### 🔰 Assignment 0: Practice for Shell commands.

- Discussed about the basic commands in linux like ls, mkdir, cd, touch, grep, rm, cat etc.

---

### 🔰 Assignment 1: Shell programming Write a program to implement an address book with options given below: a) Create address book. b) Viewaddress book. c) Insert a record. d) Delete a record. e) Modify a record. f) Exit.

- Created a menu drived program to do operations on database using shell scripting.
- program allows user to perform all CRUD operations.
- Linux system colors are used to show warnings, success messages and errors.
- Email address is used as a Primary key

---

### 🔰 Assignment 2: The demonstration of FORK, EXECVE and WAIT system calls along with zombie and orphan states. Implement the C program in which the main program accepts an integer array. Main program uses the FORK system call to create a new process called a child process. Parent process sorts an integer array and passes the sorted array to the child process through the command line arguments of EXECVE system call. The child process uses EXECVE system call to load a new program that uses.

- System calls used : fork, wait, execve
- fork : to create new process
- execve : to overlay a process image that has been created by a call to the fork function.
- wait : blocks the calling process until one of its child processes exits or a signal is received. After child process terminates, parent continues its execution after wait system call instruction.

---

### 🔰 Assignment 3: Thread management using pthread library. Implement matrix multiplication using multithreading. Application should have pthread_create, pthread_join, pthread_exit. In the program, every thread must return the value and must be collected in pthread_join in the main function. Final sum of row column multiplication must be done by the main thread (main function).

- Multiplication of matrices does take time surely. Time complexity: O(n^3)
- Strassen algorithm improves time complexity to O(n^(2.8074)).
- Multi-threading can be used to reduce this time complexity by creating
separate threads for each element in the resultant matrix.


#### pthread_create():
##### Syntax:
    int pthread_create(pthread_t *restrict thread, const pthread_attr_t *restrict attr,
    void *(*start_routine)(void *), void *restrict arg);

#### pthread_join():
##### Syntax:
    int pthread_join(pthread_t thread, void **retval);

#### pthread_exit():
##### Syntax:
    noreturn void pthread_exit(void *retval);

---

### 🔰 Assignment 4: Thread synchronization using counting semaphores and mutual exclusion using mutex. Application to demonstrate: producer-consumer problem with counting semaphores and mutex.

#### Producer Consumer Problem:

- It is an example of a multi-process synchronization problem.
- The producer and the consumer share a common fixed-size buffer
memory.
- The producer’s job is to generate data, put it into the buffer, and start
again
- At the same time, the consumer is consuming the data (i.e.,
removing it from the buffer), one piece at a time.

---

### 🔰 Assignment 5: Reader Writer Problem solution with Mutex, Semaphore.

#### Functions for semaphore :

– wait() : decrements the semaphore value.
– signal() : increments the semaphore value.

#### Writer process:
- Writer requests the entry to the critical section.
- If allowed i.e. wait() gives a true value, it enters and performs the write. If
not allowed, it keeps on waiting.
- It exits the critical section.

#### Reader process:
- Reader requests the entry to the critical section.
- If allowed:
    - it increments the count of the number of readers inside the critical
      section. If this reader is the first reader entering, it locks the wrt
      semaphore to restrict the entry of writers if any reader is inside. -
    - It then signals mutex as any other reader is allowed to enter while
      others are already reading.
    - After performing reading, it exits the critical section. When exiting, it
      checks if no more reader is inside, it signals the semaphore “wrt” as
      now, the writer can enter the critical section.
 - If not allowed, it keeps on waiting.

---

### 🔰 Assignment 6: Implement the deadlock-free solution to Dining Philosophers problem to illustrate the problem of deadlock and/or starvation that can occur when many synchronized threads are competing for limited resources.

- Problem description along with the code is given in the pdf.

---

### 🔰 Assignment 7: Inter process communication in Linux using Pipes: Full duplex communication between parent and child processes. Parent process writes a pathname of a file (the contents of the file are desired) on one pipe to be read by the child process and the child process writes the contents of the file on the second pipe to be read by the parent process and displays on standard output.

- Problem description along with the code is given in the pdf.
---

### 🔰 Assignment 8: Inter-process Communication using Shared Memory using System V. Application to demonstrate: Client and Server Programs in which the server process creates a shared memory segment and writes the message to the shared memory segment. Client process reads the message from the shared memory segment and displays it to the screen.

- Problem description along with the code is given in the pdf.
---


### You can find in me in the web 🌍
[<img align="left" alt="chaitanya-uge | LinkedIn" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg" />][linkedin]
[<img align="left" alt="chaitanya1 | Medium" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/medium.svg" />][medium]
[<img align="left" alt="chaitanya-uge | Instagram" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/instagram.svg" />][instagram]
[<img align="left" alt="chaitanyauge | Twitter" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/twitter.svg" />][twitter]

<br/>

---
[twitter]: https://twitter.com/ChaitanyaUge
[instagram]: https://www.instagram.com/chaitanya-uge/
[linkedin]: https://www.linkedin.com/in/chaitanyauge/
[medium]: https://medium.com/@chaitanya1/
