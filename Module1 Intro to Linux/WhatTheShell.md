# What The Shell
So now we know what Linux is. Additionally, we know that Linux can be installed just about anywhere. So we have an idea of Layer 1 and 2 of an operating system, so now we should be able to move onto the few remaining layers. Lets start with a shell.

## The Terminal
In Linux, the Windows command prompt equivalent is called a terminal. This is a program that opens an interactive shell that can facilitate system calls that allow a user to interact closely with the underlying operating system. This is also where we will spend the majority of our time during this course.

There is a subtle difference between the terms *Terminal* and *Shell*
- A **Shell** is a binary that provides a user interaction with the operating system.
- A **Terminal** is the process that spawns a shell and provides a user with a shell prompt to pass requests to the attached shell process

## Types of shells

Each Linux Distribution comes with their own preferred shell binary. The differences of shells are subtle but still important to recognize. 

When you open an instance of a Terminal you will be met with something similar to below

**Picture of Terminal Here**

The binaries for most shells can be found in the /bin directory. Most modern shells are based off of the `Bourne Shell` which still comes out of the box with most Linux distributions. 