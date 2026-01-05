

# Process Management Commands

## 1. Kill a Process Immediately
```bash
kill -9 <pid>
````

* Forcefully stops a process.
* The process is terminated immediately without cleanup.
* Use only when the process does not respond to normal signals.

## 2. Take a Thread Dump (for Developers)

```bash
kill -3 <pid>
```

* Used when a developer asks for a **thread dump** of a running process.
* Safely generates thread dump information (commonly for JVM processes).
* Helps developers analyze:

  * Which threads are running or blocked
  * Which functions or code paths are consuming more CPU
  * Deadlocks or performance bottlenecks

## 3. Temporarily Suspend a Process

```bash
kill -STOP <pid>
```

* Pauses (suspends) a running process without terminating it.
* The process can be resumed later using:

```bash
kill -CONT <pid>
```

## 4. List the services running in a linux machine

```bash
systemctl list-unit --type=service
```

* This command will list all the services running on a linux server.

<img width="959" height="351" alt="image" src="https://github.com/user-attachments/assets/30b6d19b-e12b-490d-92e9-6dbf2e80943c" />

## Services vs Process
* Services are a special kind of process that start upon booting of a server, whenever a server restarts the service starts up automatically but it is not the same with process

