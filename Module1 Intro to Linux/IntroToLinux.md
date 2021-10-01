# Intro to Linux

Now that we have an understanding of what an operating system is as well as an idea of what segments of an operating system perform what operations, where does the word Linux fit into this mix?

## What is Linux?

Linux is a kernel developed by Linus Torvalds in 1991 as an open source alternative to the MINIX kernel. This means a couple things that are important to note.

1.  Linux had undergone about 20 years of development in addition to the baseline Unix foundations
2.  Linux is a kernel, not an operating system
3.  Linux is open source

### Linux Development

The major source for Linux development is major contributions of the Free Software Foundation and the GNU Project. Since its beginning, the source code for the Linux kernel has been available to modify and redistribute absolutely free. Over the course of its lifetime, developers and security researchers from around the world have contributed to the development of the Linux kernel to continue to make it both a modern and secure alternative to proprietary kernels.

### Open Source Software

Open source software is software that has its source code freely accessible to anyone. Period. This means, if you'd like to build a Linux based operating system you have all of the tools available to you. If you've like to research exactly how a driver interacts with a system or process then you can go right ahead. If there's some arbitrary security concept that you'd like to learn more about and need an example, then Linux might be where you go for it! Absolutely nothing is hidden from users with regards to the Linux kernel.

However, this doesn't necessarily mean that software or operating systems that utilize or are based on the Linux kernel are all open sourced. Its possible for an operating system or critical operating system software (like a driver) utilizing the Linux kernel to be proprietary to the developers of a product assuming its not a direct copy / paste of the Linux kernel. Because Linux is under the GNU General Public License (GPL) this means that the Linux kernel cannot be redistributed in proprietary software, but it can be the inspiration for alterations of the Linux kernel and provide a solid foundation for anyone hoping to do research into the anatomy of kernels.

The benefit of open source software is, because the source code is freely accessible to everyone, this also includes security researchers and developers. The contributions of the world has helped operating systems utilizing the Linux kernel to on average be more stable, lightweight, and secure than other proprietary operating systems.

### Linux Kernel

One of the things you might be ready to move onto up to this point is "downloading Linux" and if you're interested in a freestanding kernel then by all means hit that download button! However, without any hardware for the kernel to interact with or any shell to then interact with the kernel it becomes a rather useless bit of storage.

If you remember in the previous lesson, an operating system is a construct made up of several pieces, some visible and some invisible to a user. In order to make an operating system work, we will need more than just a kernel. This is where the many "flavors" or distributions of Linux come in.

## Linux Distributions

The flexibility of Linux based operating systems lies in the tool sets that come as a part of the package with the operating system. Instead of being a general purpose operating system like windows, Linux based operating systems are a tool with purposes designated by the developers that can be altered and molded to exactly what a user's desired experience is. For example

- Kali Linux is a Debian based operating system designed and maintained by Offensive Security that runs on a Linux kernel. Kali Linux is designed to be an operating centered around the concept of security research. Many tools that come out of the box with this distribution are tools commonly used by both malicious and ethical hackers in their operations.
- Ubuntu Server is a lightweight Debian based operating system with no GUI. The lack of a GUI in the operating system makes for less points of potential failure and wear on the hardware over long periods of time. This means that systems running this operating system can run for years without ever needing to be turned off or restarted, all while providing a stable user experience.
- Android OS is based off of Linux and also participates in their own open source project. Because of the edits made by Google as well as the original developers of Android, the operating system is now the most popular mobile OS in the world. 
- Operating systems for embedded systems or the Internet of Things are predominantly based off of some version of a bare bones Linux based operating system. Because of constant security updates, the ability to freely edit, and the overall light weight of the Linux kernel, this is a go to choice for any developers of some machine that requires basic computing functionality.

In addition to each of the unique flavors and features that each Linux distribution has, it should be noted that through copious edits each operating system can have the same functionality as any other one. There is nothing preventing a user from turning their personal Ubuntu machine into a hacking machine by downloading the same tools that Kali Linux has. You are only limited by your creativity when it comes to the development of your Linux environment.