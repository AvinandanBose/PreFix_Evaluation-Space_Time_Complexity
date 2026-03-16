# Prefix Evaluation: Space & Time Complexity Analysis

![GitHub repo size](https://img.shields.io/github/repo-size/AvinandanBose/PreFix_Evaluation-Space_Time_Complexity)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

## 📌 About The Repository
This repository covers everything about **Prefix Evaluation**, breaking down how these expressions are processed at both logical and hardware levels. It includes detailed PDF notes on hardware memory mechanisms, operation steps, and thorough analyses of space and time complexities.

## 📂 Topics & Resources Included

The repository features comprehensive PDF guides covering the following concepts:

* **Prefix Evaluation Concepts:** Core mechanisms of evaluating prefix expressions.
* **PUSH Mechanism:** Hardware memory mechanism when interacting with the stack.
* **Operation Mechanism:** How mathematical operations happen in hardware memory.
* **POP Instructions:** Comparing Logical (Programmed) POP vs. Hardware Instruction POP.
* **Array Address Calculation:** Hardware mechanism for calculating array bounds (`BaseAddress + index × SizeOf(DataType)`).
* **[Extra] ENDL and ASCII:** Hardware mechanisms regarding line breaks and ASCII formats.
* **Memory Clarification:** Deep dive into Memory READ and WRITE (Magnetic Core vs. Modern RAM-CPU).
* **Complexity Analysis:** Breakdown of Space and Time Complexities for Prefix Evaluation.

## ⏱️ Time Complexity Analysis: `O(n)`

Evaluating a prefix expression involves processing the characters and using a stack.

* The primary operation involves traversing the prefix string. If the string has length `n`, scanning it takes **`O(n)`** time.
* Basic arithmetic operations (`+`, `-`, `*`, `/`, `%`, `^`) take constant time: **`O(1)`** each.
* The `push` and `pop` stack operations also take constant time: **`O(1)`** each.
* Executing the switch-case logic across the entire expression operates `O(n)` times overall.
* Returning the final popped element takes **`O(1)`** time.
* **Total Time Complexity = `O(1) + O(n) + O(n) + O(1) + O(1) + O(n) + O(1) = O(n)`**, where `n` is the length of the prefix string.

## 💾 Space Complexity Analysis: `O(n)`

The space complexity is determined by the maximum size of the stack during execution.

* Pushing operands to the stack requires auxiliary space. In the worst-case scenario, the stack needs to hold a number of elements proportional to the length of the expression.
* This stack usage requires **`n`** auxiliary space.
* **Total Space Complexity = `O(n)`**, where `n` is the size of the stack or length of the expression.

## 💻 Code Implementation

If you are looking for the actual C++ code to implement Prefix Evaluation, check out the following repository:
👉 **[C++ - Data Structures Repository](https://github.com/AvinandanBose/CPLUSPLUS_DataStructure)**

## 📜 License
This repository is licensed under the [MIT License](LICENSE).
