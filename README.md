# Unix Command-Line Systems Toolkit

A **systems-focused Unix/Linux command-line project** demonstrating how core OS utilities and shell semantics can be composed to perform reliable, efficient file system and text-processing operations in production-like environments.

The project emphasizes **tool-based problem solving, correctness, and composability**, reflecting workflows used in backend, infrastructure, and systems engineering.

---

## 🔍 Overview

This repository implements and validates a collection of Unix command-line workflows that replicate common tasks in Linux-based development environments:

* File system manipulation and traversal
* Permission and access control management
* Stream-based text processing
* Pattern matching with regular expressions
* Pipeline construction and I/O redirection
* Exit-code–driven execution control

All functionality is implemented using **standard Unix utilities and Bash**, without custom scripts or external dependencies.

---

## 🧠 Systems Design & Execution Model

### Command Composition

* Commands are composed using **pipes** to form deterministic data-processing pipelines
* Standard input/output streams are used to eliminate unnecessary intermediate files
* Each command is treated as a single-responsibility system component

This mirrors the Unix philosophy used extensively in production tooling and automation.

---

### File System Semantics

The project exercises core file system behaviors, including:

* Relative vs absolute path resolution
* Recursive operations and directory traversal
* Safe handling of non-existent or restricted resources
* Metadata inspection and verification

These operations model real-world workflows in build systems, deployment pipelines, and server environments.

---

### Permissions & Access Control

* Explicit manipulation of read, write, and execute permissions
* Understanding numeric and symbolic permission modes
* Observing how permission changes affect runtime behavior

This demonstrates practical knowledge of multi-user system security and access boundaries.

---

## 🔎 Text Processing & Data Querying

Structured text is queried and transformed using:

* `grep` / `egrep` with precise regular expressions
* Field-based extraction using `cut`
* Ordering and deduplication using `sort` and `uniq`
* Quantitative analysis using `wc`

The project demonstrates how non-trivial data analysis can be performed efficiently without bespoke code.

---

## 🔄 Validation & Correctness

Correctness is enforced through:

* File comparison using `cmp` and `diff`
* Explicit inspection of process exit codes
* Deterministic output verification

These practices reflect defensive engineering and reliable system interaction.

---

## ⚙️ Shell Semantics & Control Flow

The project demonstrates mastery of core shell behaviors:

* Input/output redirection
* Wildcard expansion and quoting rules
* Command substitution
* Conditional execution using logical operators (`&&`, `||`)

This ensures predictable behavior in complex command sequences.

---

## 🛠️ Technologies & Concepts

* **Environment:** Unix / Linux
* **Shell:** Bash
* **Tooling:** Core GNU utilities
* **Core Concepts:**

  * Unix philosophy
  * File system abstractions
  * Permissions and access control
  * Stream processing
  * Regular expressions
  * Exit codes and error handling

---

## 🚀 Why This Project Matters

This project demonstrates competencies directly relevant to **FAANG-scale software engineering**:

* Systems-level thinking using real OS primitives
* Precision and correctness in tooling-based workflows
* Strong understanding of Linux execution models
* Ability to build reliable, composable solutions from low-level components
* Comfort operating close to the operating system boundary

---

## 👤 Author

**Computer Science (Honors)**  
York University  
Third-Year Computer Science Honors Student
