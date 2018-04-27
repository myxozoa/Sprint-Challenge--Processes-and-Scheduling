### List all of the main states a process may be in at any point in time on a standard Unix system. Briefly explain what each of these states mean.

-----

*Running: the process is running
*Interruptible: waiting for a signal from another process
*Uninterruptible: waiting for a hardware state
*Stopped: process is stopped
*Zombie: the process has finished/terminated but still exists in the process table
*Orphan: the process's parent process has finished/terminated before itself

### What is a Zombie Process? How does it get created? How does it get destroyed?

-----

A child process becomes a zombie after finishing completion, so that the parent can read it's exit status.  It is reaped by the system.

### Describe the job of the Scheduler in the OS in general.

-----

To organize and give execution time as fairly as possible to every running process.

### Describe the benefits of the MLFQ over a plain Round-Robin scheduler.

-----

An MLFQ can generate much better response times/latency for a better user experience, and shorter processes are inherently preferred by an MLFQ without adjusting the time quantum.