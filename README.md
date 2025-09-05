# Basic Computer Information
# Computer Science & Hardware Notes

## 1. Types of Memory and Storage

### Memory (Volatile)
* **RAM (Random Access Memory)**
    * **SRAM (Static RAM):** Faster than DRAM. Used for CPU caches.
    * **DRAM (Dynamic RAM):**
        * SDRAM
        * DDR SDRAM (e.g., DDR4, DDR5)
        * GDDR SDRAM (For graphics cards)
* **ROM (Read-Only Memory)** (Non-Volatile)
    * Firmware
    * BIOS

### Storage (Non-Volatile)
* HDD (Hard Disk Drive)
* SSD (Solid State Drive)
* USB Drive
* SD Card

---

## 2. Processing Units (CPU, GPU, TPU)

### Core Differences
* **CPU (Central Processing Unit):**
    * **Compute Primitive:** Scalar (single value).
    * **Operation:** Parallelized scalar multiplication.
    * **Memory Management:** Implicitly managed (L1, L2, L3 caches).
* **GPU (Graphics Processing Unit):**
    * **Compute Primitive:** Vector (1D array).
    * **Operation:** Parallelized vector multiplication.
    * **Memory Management:** Mixed (L1, L2 caches, Shared Memory).
* **TPU (Tensor Processing Unit):**
    * **Compute Primitive:** Tensor/Matrix (2D array).
    * **Operation:** Parallelized matrix multiplication.
    * **Memory Management:** Explicitly managed (Activation Buffer, Register File).

### Other Processing Hardware
* **APU (Accelerated Processing Unit):** CPU and GPU on a single chip.
* **FPGA (Field-Programmable Gate Array):** Reconfigurable integrated circuit.
* **AI Accelerators:** Specialized hardware for AI workloads.
* **RISC-V:** An open-source instruction set architecture (ISA).

---

## 3. Major Fields of Computer Science

### Theoretical Computer Science
* Algorithms & Complexity
* Computability Theory
* Information Theory & Cryptography

### Computer Engineering
* Computer Architecture
* Hardware (CPU, RAM, Motherboard)
* Operating Systems
* Programming Languages & Compilers

### Applications
* Artificial Intelligence (Machine Learning, NLP, Computer Vision)
* Robotics
* Big Data
* Virtual & Augmented Reality
* Internet of Things (IoT)
# Computer Science & Systems Notes

## Linux Filesystem Hierarchy

* `/`: **Root** directory.
* `/bin`: Essential user **binaries**.
* `/sbin`: Essential **system** binaries (for admins).
* `/etc`: System-wide **configuration** files.
* `/dev`: **Device** files.
* `/home`: **User** home directories.
* `/lib`: Essential shared **libraries**.
* `/var`: **Variable** files (logs, caches).
* `/tmp`: **Temporary** files.
* `/usr`: User programs and data.
* `/boot`: **Boot** loader files.
* `/opt`: **Optional** application software.
* `/mnt`: Temporary **mount** point.
* `/media`: Mount point for **removable devices**.

---

## Memory & Storage Hierarchy

A trade-off from faster/smaller/costlier to slower/larger/cheaper.

1.  **Registers:** On-CPU, fastest.
2.  **Cache (L1, L2, L3):** On-CPU, very fast.
3.  **RAM (DRAM):** Main memory.
4.  **SSD (Solid State Drive):** Fast storage.
5.  **HDD (Hard Disk Drive):** Slowest storage.

---

## OSI Networking Model

* **Software Layers**
    * 7. **Application Layer:** User-facing protocols (HTTP, SMTP).
    * 6. **Presentation Layer:** Data translation, encryption, compression.
    * 5. **Session Layer:** Manages connections.
* **Transport Layer**
    * 4. **Transport Layer:** End-to-end communication (TCP, UDP).
* **Hardware Layers**
    * 3. **Network Layer:** Packet routing (IP).
    * 2. **Data Link Layer:** Framing and physical addressing (MAC).
    * 1. **Physical Layer:** Raw bit transmission (cables, hardware).

---

## Programming Language Performance

Performance generally depends on the execution type.

* **Most Efficient (Compiled):**
    * C, Rust, C++.
    * Low energy, time, and memory usage.
* **Moderately Efficient (VM/Compiled):**
    * Ada, Java, Go, C#.
* **Least Efficient (Interpreted):**
    * Python, Ruby, Perl, Lua.
    * High energy, time, and memory usage.
      # introduction to python
      # Python & Data Structures Notes

## Python Learning Roadmap

### 1. Basics
* Basic Syntax
* Variables & Data Types
* Conditionals (if/else)
* Loops (for, while)
* Functions
* Exceptions
* Built-in Data Structures (Lists, Tuples, Sets, Dictionaries)

### 2. Data Structures & Algorithms (DSA)
* Arrays & Linked Lists
* Heaps, Stacks, Queues
* Hash Tables
* Binary Search Trees
* Recursion
* Sorting Algorithms

### 3. Object-Oriented Programming (OOP)
* Classes
* Methods
* Inheritance

### 4. Advanced Topics
* List Comprehensions
* Generators & Iterators
* Decorators
* Lambdas
* Regular Expressions (Regex)
* Threading
* Functional Programming (map, reduce, filter)

### 5. Specializations
* **Web Frameworks:** Django, Flask, FastAPI
* **Data Science:** NumPy, Pandas, Matplotlib, Scikit-learn, TensorFlow, PyTorch
* **Automation:** Web Scraping, File Manipulation, GUI Automation
* **Testing:** Unit Testing, Integration Testing, End-to-end Testing
* **Version Control:** Git, GitHub/GitLab
* **Package Managers:** pip, conda

---

## Data Structures Overview

### 1. Primitive Types
* Integer
* Float
* String
* Boolean

### 2. Non-Primitive Types

#### Python Built-in
* **List:** Ordered, mutable, indexed. Created with `[]`.
* **Tuple:** Ordered, immutable.
* **Dictionary:** Unordered (in older Python), key-value pairs.
* **Set:** Unordered, unique elements.

#### User-Defined / Abstract
* **Linear**
    * Stack
    * Queue
    * Linked List
* **Non-Linear**
    * Tree
    * Graph
    * Hash Table
    * # Programming Quick Notes

## Python

### How it Works
* **Source Code (`.py`)** -> Compiler -> **Bytecode (`.pyc`)**
* **Bytecode** -> Python Virtual Machine (PVM) -> Interpreter -> **Machine Code**
* **Result:** Running Program

### Core Concepts
* **Data Types:** Lists, Numeric, Text.
* **Operators:** Arithmetic, Assignment, Comparison, Logical.
* **Strings:** Single-line, Multi-line, Raw, Unicode.
* **Conditions:** Control program flow.
* **Functions:** Built-in, User-defined, Lambda, Recursive, Higher-order, Generator.

### Data Structures
* **Tuples:** Immutable Arrays.
* **Lists:** Mutable Arrays.
* **Dict:** Hashtables (Key-Value Pairs).

---

## C Compilation Process

1.  **Preprocessor:** `.c` file -> `.i` file (Handles includes).
2.  **Compiler:** `.i` file -> `.s` file (Creates Assembly Code).
3.  **Assembler:** `.s` file -> `.obj` file (Creates Object Code).
4.  **Linker:** `.obj` file + Libraries -> `.exe` file (Creates Executable).

---

## OOP Concept: Encapsulation

* **Definition:** Bundling data (variables) and methods (functions) together inside a **Class**.
* **Purpose:** Hides internal state and requires interaction through methods.
* # Programming Quick Notes

## OS Concepts

### Program vs Process vs Thread
* **Program:** Executable file stored on Disk (e.g., an `.exe` or `.app` file).
* **Process:** A program in execution, loaded into RAM (Memory).
* **Thread:** A single, sequential flow of execution within a Process. A process can have multiple threads.

---

## Data Structures

* **Linear Data Structures:** Data elements are arranged sequentially.
    * Array
    * Stack
    * Queue
    * Linked-list
* **Non-linear Data Structures:** Data elements are arranged in a hierarchical manner.
    * Graphs
    * Trees

---

## OOP Concepts

* Class
* Object
* Inheritance
* Polymorphism
* Abstraction
* Encapsulation

---

## Python Notes

### Python Functions

* **Normal Function:** A reusable block of code defined with the `def` keyword.
    * Syntax: `def function_name(parameters):`
    * Contains a function body and can have a `return` statement.
* **Lambda Function:** A small, anonymous function defined with the `lambda` keyword.
    * Can have multiple arguments but only one expression.
    * Syntax: `variable = lambda parameters: expression`

### Common Functions & Keywords

* `print()`: Display output.
* `len()`: Get length.
* `input()`: Get user input.
* `range()`: Generate a sequence of numbers.
* `str()`, `int()`, `float()`: Convert data types.
* `list()`, `dict()`: Create list or dictionary.
* `if...else`: Conditional execution.
