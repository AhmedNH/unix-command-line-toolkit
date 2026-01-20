# Unix Command-Line Systems Toolkit

This project showcases **practical Unix/Linux command-line proficiency**, demonstrating how core system utilities and shell features can be composed to solve real-world file system, text-processing, and automation tasks efficiently.

The focus is on **tool-based problem solving**, leveraging standard Unix utilities and shell semantics rather than graphical interfaces.

---

## 🔍 Overview

The repository contains a collection of workflows and command sequences that replicate common tasks performed in Linux-based development and server environments, including:

* File and directory manipulation
* Permission and ownership management
* Text processing and comparison
* Pattern matching with regular expressions
* Command pipelines and redirection
* Exit-code–driven control flow

All tasks are completed using **standard Unix utilities**, emphasizing correctness, composability, and efficiency.

---

## 🧠 System-Level Concepts

### Command Composition & Pipelines

The project demonstrates how small, single-purpose tools can be composed using pipes to form powerful workflows:

* Chaining commands to process data streams
* Avoiding intermediate files where possible
* Leveraging standard input/output semantics

This reflects the Unix philosophy of building complex behavior from simple primitives.

---

### File System Operations

Operations performed include:

* Creating, copying, moving, renaming, and deleting files and directories
* Recursive directory traversal
* Relative vs absolute path resolution
* Safe handling of non-existent files and directories

These workflows mirror tasks commonly encountered in development, deployment, and debugging environments.

---

### Permissions & Access Control

The project explores Unix file permissions in depth:

* Read, write, and execute modes
* Numeric and symbolic permission representations
* Understanding how permissions affect program execution and file access

This provides insight into access control and security fundamentals in multi-user systems.

---

## 🔎 Text Processing & Search

A significant portion of the project focuses on extracting and transforming structured text data using:

* `grep` / `egrep` with regular expressions
* `sort`, `uniq`, and field-based ordering
* `cut` for column extraction
* `wc` for quantitative analysis

These tools are used to perform non-trivial data queries without writing custom programs, showcasing efficiency and precision.

---

## 🔄 Validation & Correctness

To ensure correctness:

* File comparisons are validated using `cmp` and `diff`
* Exit codes are explicitly checked to verify command success or failure
* Outputs are inspected for deterministic behavior

This reinforces defensive workflows and reliable system interaction.

---

## ⚙️ Shell Features & Execution Model

The project demonstrates core shell behaviors, including:

* Input and output redirection
* Wildcards and filename expansion
* Command substitution
* Conditional execution using logical operators (`&&`, `||`)
* Quoting rules and their effects on evaluation

Understanding these behaviors is critical for writing safe and predictable shell commands.

---

## 🛠️ Technologies & Concepts

* **Environment:** Unix / Linux
* **Shell:** Bash
* **Utilities:**

  * Core GNU utilities (`ls`, `cp`, `mv`, `rm`, `chmod`, `find`, etc.)
  * Text-processing tools (`grep`, `sort`, `uniq`, `cut`)
* **Core Concepts:**

  * Unix philosophy
  * File system abstractions
  * Permissions and access control
  * Stream-based processing
  * Regular expressions
  * Exit codes and error handling

---

## 🚀 Why This Project Matters

This project demonstrates skills directly applicable to **software engineering internships**:

* Comfort working in Linux-based environments
* Ability to reason about systems through tooling
* Writing precise, efficient command-line workflows
* Understanding how programs interact with the OS
* Translating abstract system concepts into concrete operations

These skills are essential for backend development, DevOps, infrastructure, and systems-focused roles.

---

## 👤 Author

**Computer Science (Honours)**  
York University  
Third-Year Computer Science Honors Student
