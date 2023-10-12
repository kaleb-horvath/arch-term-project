1. Research and understand LC3 architecture. Should be be able to
   * Acquire both the implementation and assembler
   * Write simple programs in LC3 assembly (see Col-State practice assignments, this could include useful subroutines that would apply to writing a simple OS)
     * Software stack implementation 
     * Block allocation routines
     * Simple ADT implementations 
     * Exercises (Project Euler questions, etc.)
   * Study source code of chosen implementation (of LC3) 
     * Understand each function 
     * Diagram instruction pipeline (ID, IF, EX, WB)
     * Pursue possible optimizations (low priority)
     * Understand addressing modes and address translation 
     * Understand I/O as it exists by default in the chosen implementation. Start to think about how we will apply this to our use-case, that is getting physical hardware devices to talk to the LC3
   * Build/find debugger
     * Should show status of memory locations and registers during program execution
     * Should show current instruction being executed
     * Should indicate current stack frame
2. Research and understand previous attempts to develop LC3 operating systems
   * Take note of various strategies used to solve different problems 
   * Take note of service routine and I/O setup 
   * Take note of any usage of a software stack and pre-written routines 
3. Begin development of LC3 OS capable of meeting requirements enumerated in project Abstract 
4. Build serial display and character input device
   * Wire to micro controller, verify data can be read/written via serial cable to an from micro controller from host system running LC3
   * Write Python or C program to
     * Buffered reader and writer to hardware devices
     * Handle character encoding
     * Translate/move data to LC3 address space and from micro controller serial-I/O address space on host system 
   * Implement blocked/buffered IO routines (outside of general service routines that will come with the OS) to read from the designated serial IO address space inside of the LC3 program 
     * These should be specially designed to handle reading and writing characters to the display and input device 
     * UNIX-like concept of representing hardware devices as files?
       * FD, Open, Read, Write, etc. 
       * Handling multiple characters in a single read/write?
       * Does this require a data structure implementation? 
5. Lisp compiler!



