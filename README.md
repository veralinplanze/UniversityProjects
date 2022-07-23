# Consumer-Producer thread problem
Thread MVC model with 2 consumers and 1 producer. The task is to produce some amount of processes, which will take place in a buffer container(it can store 1 process at time), 2 CPUs, as consumers, will take created process and immitate some work with it. By the time new process is created, if the old one is not taken by any of 2 processors, it replaces the old one (destroys it). The task is to calculate statistics of destroyed and served processes for each CPU. Current version is not working as intended, because monitor doesn`t wrap the right part of code, which is needed to be synchonized, so it causes consumers to take "null processes" from a buffer. But since it has no runtime errors, I took this as a success start of my first multithread program.
