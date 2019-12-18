# Numba

## Introduction to Numba (CUDA)

Welcome to this notebook about Numba !!

Numba is a Python compiler, specifically for numerical functions and allows you to accelerate your applications with high performance functions written directly in Python.

Numba generates machine code optimized from pure Python code using LLVM. With a couple of simple changes, our Python code (function-oriented) can be optimized "just-in-time" to obtain a performance similar to that of C, C ++, without having to change the language.

## What is Numba?
Numba is a compiler that allows you to accelerate Python code (numerical functions) for both CPU and GPU:

1. Function Compiler: Numba compiles Python functions, not whole applications or parts of it. Basically, Numba is another Python module to improve the performance of our functions.

2. Just-in-time: (Dynamic translation) Numba translates the bytecode (intermediate code more abstract than the machine code) to machine code immediately before its execution to improve the execution speed.

3. Numerically-focused: Numba is focused on numerical data, such as int, float, complex. For now, there are limitations to use it with string data.

Numba is not the only way to program in CUDA, it is usually programmed in C / C ++ directly for it. But Numba allows you to program directly in Python and optimize it for both CPU and GPU with few changes in our code. In relation to Python, there are other alternatives such as pyCUDA, here is a comparison between them:

### CUDA C / C ++:

- It is the most common and flexible way to program in CUDA
- Accelerate applications in C, C ++.

### pyCUDA

- It is the most efficient CUDA form for Python
- It requires programming C in our Python code and, in general, many code modifications.

### Numba

- Less efficient than pyCUDA
- It allows you to write your code in Python and optimize it with few modifications
- It also optimizes the Python code for CPU
