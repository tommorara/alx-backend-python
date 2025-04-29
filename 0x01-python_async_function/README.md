# 0x01. Python - Async

## 📚 Project Overview
This project focuses on **asynchronous programming in Python**. It introduces key concepts such as `async`/`await` syntax, concurrent coroutine execution with `asyncio`, creating tasks, and measuring runtime performance.  
By the end, you should be able to confidently explain and apply asynchronous patterns in Python without external help.

---

## ✨ Learning Objectives
At the end of this project, you will be able to:

- Understand and use `async` and `await` syntax
- Execute asynchronous programs using the `asyncio` library
- Run multiple coroutines concurrently
- Create and manage asyncio tasks
- Utilize the `random` module for introducing randomness in delays

---

## 📋 Requirements
- A `README.md` file is mandatory at the project root.
- Allowed editors: `vi`, `vim`, `emacs`
- All files will be interpreted/compiled on **Ubuntu 18.04 LTS** with **Python 3.7**
- Code must comply with **pycodestyle** (version 2.5.x)
- Files must end with a new line and be executable.
- The first line of each Python file must be:
  ```bash
  #!/usr/bin/env python3
  ```
- All functions and coroutines must include **type annotations**.
- Every module and function must include a **full documentation string** explaining its purpose.

---

## 🧩 Tasks

### 0. The basics of async
- Create an asynchronous coroutine `wait_random`.
- Takes an integer `max_delay` (default: `10`).
- Waits for a random delay between `0` and `max_delay` seconds.
- Returns the random delay.

📄 File: `0-basic_async_syntax.py`

---

### 1. Execute multiple coroutines concurrently
- Create an async routine `wait_n`.
- Spawns `wait_random` `n` times with the specified `max_delay`.
- Returns a list of all delays, sorted in ascending order.

📄 File: `1-concurrent_coroutines.py`

---

### 2. Measure runtime
- Create a function `measure_time`.
- Calculates the average time per execution of `wait_n(n, max_delay)`.

📄 File: `2-measure_runtime.py`

---

### 3. Create tasks
- Create a regular function `task_wait_random`.
- Returns an `asyncio.Task` object that wraps `wait_random`.

📄 File: `3-tasks.py`

---

### 4. Concurrent tasks
- Create an async routine `task_wait_n`.
- Similar to `wait_n`, but uses `task_wait_random` instead of directly awaiting `wait_random`.

📄 File: `4-tasks.py`

---

## 🛠️ Resources
- [Async IO in Python: A Complete Walkthrough](https://realpython.com/async-io-python/)
- [asyncio — Asynchronous I/O documentation](https://docs.python.org/3/library/asyncio.html)
- [random.uniform function documentation](https://docs.python.org/3/library/random.html#random.uniform)

---

## 📜 Repository
- GitHub repository: **alx-backend-python**
- Directory: **0x01-python_async_function**

---

## ©️ Copyright
