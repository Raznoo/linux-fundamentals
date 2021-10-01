## What is a Computer

In the most basic sense, a computer is a very long series of complicated circuits that perform operations extraordinarily fast. As a review from the IT Fundamentals Course, the basic order of operations for a program being loaded is...
1. A file is loaded onto memory from some storage
2. The CPU will look for a section of memory to begin execution of the program
3. The CPU will execute the instruction currently pointed to in memory 
	- The instruction address is pointed to and stored by registers
4. Operations are executed by the CPU and any other required hardware
5. Results of operation are stored, shown, or some phsycial action takes place
	- Disk tray opening, fan turning on, monitor changing pixel, etc.
6. Step repeats for each instruction stored in memory
7. Exit program

In theory, this sounds like a graceful solution to many very difficult issues for automating mundane tasks where accuracy was important. In roles that requires many simple operations, a computer made alot of sense. and before the 21st century, this was an accepted approach to computing. 

However, as hardware became more complicated, so did their processes. Computer Engineers began moving away from programs on punch cards and floppy disks and began storing them on magnetic hard disk drives. In addition to the digital abstraction of a file system, processors began being able to run two or three programs at the same time. Error checking and crash reports became more common for debugging and technological development. 

But how are all of these systems managed? What tells a computer to go from step 1 to step 2 in the above sequence? What actually determines what qualifies as an error?

## What is an Operating System
The answer is an operating system. 

An operating system is an abstraction that simply is the method by which a manufacturer has decided to handle computing processes like virtualization, resource management, file storage, etc. 

Some common modern operating systems include
- Windows 10
- Ubuntu
- Kali Linux
- MacOS

Each of the manufacturers above have a concept for default configurations, how to manage resources, software that comes by default on a system, and more. For instance, MacOS by default comes with other Apple software like iTunes whereas Windows systems come with other Microsoft software like the Microsoft Store.

How an operating system manages resources and configurations is beyond the scope of this course. However, we will build an abstraction for the layers of an operating system. 

## Layers of an OS

### Layer 1 Hardware
This is the layer that physically stores information either by volatile means (memory and caches) or with more stable means (storage). This is also the layer where the interactions occur for arithmetic and other operation like graphics processing. 

### Layer 2 Kernel
This layer facilitates any calls for the utilization of hardware. Any request to read from, write to, or execute an instruction of memory needs to go through the kernel. This is the most privileged space that a user can interact with as all hardware operations are done as a system request through the kernel.

### Layer 3 Shell
An easy way to view this layer is thinking of it as the command prompt in Windows and the terminal in Linux based operating systems. While there are other ways to utilize interactions with a shell, these are the most common.

A shell is any program or process that can create or make system calls to the kernel. In command lines this is done by using commands to read, write, or execute files, or by sending signals for operating system commands like the `shutdown` command.

### Layer 4 User Land (Application)
This is the safe zone for guests or non admin users. This is usually a restricted environment that has the ability to request actions from a restricted user shell to then perform operating system commands. Any game you start up, and browser you open, any email you send, all happens in User Land. 

The way that processing (or anything) occurs at this layer is by utilizing binaries that the program has access to in order to utilize subsets of shell commands in order to achieve whatever required functionality a program has. 

A privileged version of User Land exists in both Windows and Linux based systems through the use of admin accounts. This mode utilizes the increased privilege of administrator users to provide access to binaries requiring admin privileges. 

Keep in mind, there is still the ability for compromise entirely contained in User Land. If you have some program that, while only existing in userland, still has access to all required shell commands, an attacker can still use a vulnerability in that program to fully compromise a system in a way that you might access your system in a way if you were sitting in front of it!