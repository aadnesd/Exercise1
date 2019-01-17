# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > *Concurrency means multiple tasks which start, run, and complete in overlapping time periods, in no specific order.
    Parallelism is when multiple tasks OR several part of a unique task literally run at the same time, e.g. on a multi-core processor.*
 
 ### Why have machines become increasingly multicore in the past decade?
 > *Difficult to increase clock frequency efficiently anymore because of heat losses, leakage current etc. 
    More cost efficient to use multi-core. Can also run multiple tasks on multiple cores**
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > *Through concurrency, programs can be designed as independent processes working together in a specific composition*
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > *Your answer here*
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > *?*
 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > *pthread_create() - thread
    threading.Thread() - thread
    go - coroutine*
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > *GIL is a mutex that protects access to python objects, preventing multiple threads from executing python bytecodes at once.
+    On multi-core systems, it means that multiple threads can't effectively make use of multiple cores.*
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > *multiprocessing*
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > *The GOMAXPROCS variable limits the number of operating system threads that can execute user-level Go code simultaneously.*
