## The Big Picture
Chapter 1 provides an overview of how Linux functions, emphasizing abstraction—a method that simplifies understanding by focusing on essential components rather than details.
## 1.1 Levels and Layers of Abstraction
•	Linux is organized into layers:
1.	Hardware – The foundation, including memory, CPU, disks, and network interfaces.
2.	Kernel – The core that manages hardware, memory, processes, and system calls.
3.	User Space – Running programs (user processes) interacting with the system.
•	The kernel operates in kernel mode (full system access), while user processes run in user mode (restricted access to prevent system crashes).

![alt text](/images/linux_org.PNG)
<br>

</br>

{:.image-caption}
*[How Linux Works, 3rd Edition]()*

<br>

</br>

## 1.2 Hardware: Understanding Main Memory
•	Main memory (RAM) stores processes and the kernel.
•	The CPU reads and writes data from memory, processing system states (arrangements of bits).
•	Virtual memory is managed by the kernel using a memory management unit (MMU).
## 1.3 The Kernel
The kernel has four main responsibilities:
1.	Process Management – Scheduling and running processes via context switching.
2.	Memory Management – Allocating and protecting memory for different processes.
3.	Device Drivers – Enabling communication between hardware and software.
4.	System Calls – Providing an interface for user programs to interact with the kernel.

<br>

</br>

![alt text](/images/system_calls.PNG)

<br>

</br>

{:.image-caption}
*[https://phoenixnap.com/kb/system-call](https://phoenixnap.com/kb/system-call)*

<br>

</br>

•	Key system calls:
-	fork() – Creates a new process.
-	exec() – Runs a new program, replacing the current process.

## 1.4 User Space
-	User space contains all running programs, organized into layers (e.g., system utilities, applications).
-	Programs may depend on system components like logging services and network configurations.
## 1.5 Users
-	Linux supports multiple users, each identified by a User ID (UID).
-	The root user (superuser) has unrestricted system access.
-	Groups allow users to share access permissions.
## 1.6 Looking Forward
-	The next chapters delve deeper into Linux components, focusing on long-term storage (disks, filesystems, etc.).

