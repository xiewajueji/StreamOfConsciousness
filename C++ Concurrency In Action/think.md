# thinking

## definition
+ Obstruction-Free -- If all other threads are paused, then any given thread will complete its operation in a bounded number of steps.
+ Lock-Free -- If multiple threads are operating on a data structure, then after a bounded number of steps one of them will complete its operation.
+ Wait-Free -- Every thread operating on a data structure will complete its operation in a bounded number of steps, even if other threads are also operating on the data structure.

one of thread running can finish while other thread blocking < 
one of thread running can finish while all thread operate on same data structure <
every thread can finish while all thread operate on same data structure

lock-free data structure can have thread starvation(aka 饿死), but wait-free don't have such problem. It presents that a thread always does a failing CAS operation.

what's the difference between hazard pointer and shared pointer?