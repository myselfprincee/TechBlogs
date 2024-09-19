---
title: "Getting into Systems Kernel and OS  - THE BEGINNING."
seoTitle: "Getting into Systems Kernel and OS  - THE BEGINNING."
seoDescription: "The kernel is the core component of an operating system. It acts as a bridge between the hardware of a computer and the software applications that run on it"
datePublished: Thu Sep 19 2024 12:32:33 GMT+0000 (Coordinated Universal Time)
cuid: cm199v1th00190ak40crkfz2v
slug: getting-into-systems-kernel-and-os-the-beginning
canonical: https://medium.com/gitconnected/getting-into-systems-kernel-and-os-the-beginning-9b19cd54b379
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1726469113469/dc02c906-8e4b-4728-b922-613de500a4d5.jpeg
tags: programming-blogs, operating-system, linux, computer-science, kernel

---

#### This word will not trouble you again.

Hello my tech geeks 👋🏻👋🏻 welcome to this blog.

Ahh, I know the title might sound technical, but don’t worry — we’re going to break it down and make it easy to understand. I’ll be here to guide you through it, and as you follow this series ( yeah, more blogs coming soon ), it will become easier and easier to grasp.

So,

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1726469161084/2ea1676b-fc19-4efe-9d05-f69cfd63a87e.png align="center")

**The kernel is the core component of an operating system. It acts as a bridge between the hardware of a computer and the software applications that run on it.**

Now if you’re new to tech or not very technical. You’re confused. you might be thinking then what is the use of CPU. everyone says it is the brain of a computer.

Here’s an analogy that will make the understanding much easier.

---

**Imagine Your Computer as a School:**

* **The CPU (Central Processing Unit)** is like the teacher in a classroom.
    
* **The Kernel** is like the principal of the school.
    

**How They Work Together:**

**The CPU (Teacher):**

* The teacher (CPU) is the one who actually teaches the students (runs programs).
    
* The teacher gives instructions, helps students solve problems, and makes sure everyone is doing their work.
    
* In computer terms, the CPU does all the “thinking” by following instructions from programs to get tasks done.
    

**The Kernel (Principal):**

* The principal (kernel) is in charge of the entire school.
    
* The principal decides which classes (programs) will run, assigns teachers (CPUs) to those classes, and makes sure everything is organized and working smoothly.
    
* The kernel tells the CPU what to do, like which program to run and when to switch between programs.
    

**Example:**

**You (Student) want to play a game (Program):**

1. You tell the principal (kernel) that you want to play a game.
    
2. The principal (kernel) tells the teacher (CPU) to start the game.
    
3. The teacher (CPU) explains the rules, makes the game work, and keeps things running smoothly.
    

In simple terms:

* **The CPU is the one that does the actual work.** It follows the instructions given to it, like teaching a lesson or running a game.
    
* **The Kernel is the manager.** It makes sure the CPU knows what to do, when to do it, and keeps everything organized.
    

Now Let’s understand the **difference between the kernel and Operating System** using the same analogy:

The **<mark>Operating System (OS)</mark>** <mark> is like the </mark> **<mark>entire school</mark>**<mark>.</mark> The **<mark>Kernel</mark>** <mark> is the </mark> **<mark>principal</mark>** ( as we know. )

---

## **The Operating System (School):**

* The whole school (OS) is where everything happens — students learn, teachers teach, and staff manages things.
    
* The school has **classrooms, hallways, a cafeteria, and rules** for how everything works (similar to the OS having apps, interfaces, and system programs).
    
* The OS includes everything the students (you) interact with — like the **classrooms** (apps), the **playground** (games), and even the **library** (file system). All these parts work together to give you a great school experience.
    
    ## **The Kernel (Principal):**
    
* The principal (kernel) manages the **whole operation of the school**.
    
* The principal decides which teachers (CPUs) will teach which subjects (programs) and when students (you) can go to different activities.
    
* The principal makes sure everything runs smoothly — whether it’s handling busy schedules, solving conflicts, or keeping the lights on (like handling memory, CPU usage, and hardware).
    

Now I think you’re ready for the standard definition that confused your mind above.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1726469208391/0800d158-6e31-4b54-919d-875a7c0c3c4a.gif align="center")

---

So, As being the Principal, The kernel has several critical responsibilities:

### **1) Resource Management:**

The kernel manages the system’s resources, such as CPU, memory, and I/O devices. It allocates these resources to different processes and ensures they are used efficiently.

### **2) Process Management:**

The kernel handles the creation, scheduling, and termination of processes (programs in execution). It ensures that multiple processes can run simultaneously (multitasking) without interfering with each other.

### **3) Memory Management:**

The kernel controls how memory is allocated to processes. It ensures that each process has access to the memory it needs while keeping processes isolated to prevent them from accessing each other’s memory space.

### **4) Device Management:**

The kernel communicates with hardware devices (e.g., hard drives, printers, network cards) through device drivers. It provides an abstraction layer so that applications can interact with hardware without needing to know the specifics of the hardware.

### **5) System Calls:**

The kernel provides a set of system calls (functions) that applications can use to request services from the operating system, such as reading a file, creating a new process, or communicating over a network.

### **6) Security and Access Control:**

The kernel enforces security policies, ensuring that users and processes have the appropriate permissions to access resources and execute commands. It helps protect the system from unauthorized access and potential threats.

<mark>More light on these points, something called protected memory space is just like using a web application which can save something in your storage but it is handled and sandboxed by chrome. like giving 5MB storage space on local storage. like this, kernel provides program, the space they require while not giving access to other processes and the storage of the application ( specifically ram ).</mark>

### **Kernels are of majorly 5 types :**

### **Micro Kernel**

A microkernel is kind of a small, modular kernel that provides only the most essential services, such as process management, memory management, and inter-process communication.

* **Advantages:** Highly modular, making it easier to add or remove features. More secure, as less code runs in privileged mode.
    
* **Disadvantages:** Can be less efficient due to the overhead of context switching between the kernel and user space.
    
* **Examples:** QNX, Mach
    

### **Monolithic Kernel**

* **Advantages:** Efficient, as it minimizes context switching between kernel and user space.
    
* **Disadvantages:** Difficult to modify or extend, as changes often require recompiling the entire kernel.
    
* **Examples:** Linux, Windows NT
    

### **Hybrid Kernel**

* A hybrid kernel combines elements of both monolithic and microkernel kernels. It provides a balance between efficiency and modularity.
    
* **Advantages:** Offers the benefits of both monolithic and microkernel kernels.
    
* **Disadvantages:** Can be complex to design and implement.
    
* **Examples:** macOS, Windows
    

### **Nano Kernel**

* **Description:** A nanokernel is an extremely small kernel, often used in embedded systems with limited resources. It provides only the most basic functions necessary for the system to operate.
    
* **Advantages:** Highly efficient and lightweight.
    
* **Disadvantages:** Limited functionality and flexibility.
    
* **Examples:** RTEMS, Nucleus
    

### **Exo Kernel**

* **Description:** An exokernel is a kernel that provides a minimal abstraction layer between hardware and applications. It allows applications to have direct control over hardware resources.
    
* **Advantages:** Highly efficient and customizable.
    
* **Disadvantages:** Complex to design and implement. Requires careful management of hardware resources.
    
* **Examples:** Singularity, Exokernel
    

---

here’s an explanation of a random keyword just for some extra knowledge.

( in the next blogs, we will be diving more and more into the kernels and OSes. so, the more knowledge, the better you will be prepared to understand that. )

### ***What is Kernel Panic?***

![](https://cdn-images-1.medium.com/max/2400/0*kBI4IbxuE8C6Vwyb.png align="left")

random image of a kernel panic

A kernel panic is a computer malfunction that the system’s operating system (OS) cannot swiftly or readily resolve. It arises when a severe, low-level error occurs, and the OS’s core component, the kernel, is incapable of resolving it.

The purpose of a kernel panic is to halt the system to prevent potential harm to the system’s software, hardware, or memory. This interruption safeguards data and permits technicians to employ a debugger for diagnosing the issue.

A kernel panic can be initiated when the operating system makes an improper effort to access or modify memory or due to software glitches and malicious software. Additional typical factors contributing to a kernel panic encompass:

* An error in the kernel itself, such as within a driver integrated into the kernel.
    
* Malfunction or incorrect installation of random access memory (RAM) modules.
    
* Hard disk impairment or data corruption.
    
* Faulty or corrupted system files, processor, or memory components.
    
* Usage of unsupported hardware.
    
* Missing or malfunctioning drives or partitions.
    
* Device drivers that are incompatible with the system.
    

---

So, that’s it for now. If you’re feeling that you’re going to forget these things. don’t worry, we will be diving more into the types of kernels which will make it easy for you to remember. ( I guarantee you won’t forget! 💯🙂 )

and if you enjoyed reading this,

Make sure to spam some hearts ( will help it reach a wider audience. )

Follow me if you want to read such content.

Subscribe to my newsletter.

and if you are very interested and want to support my work. you can [buy me a coffee too :)](https://buymeacoffee.com/princeegupta)

**bye for now 👋🏻👋🏻**

***<mark>we’ll meet again in the part II</mark>***