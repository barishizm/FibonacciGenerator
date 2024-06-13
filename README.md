# Fibonacci Series Generator

This project is a simple Python program that generates the first `n` numbers of the Fibonacci series using a recursive function.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [License](#license)

## Introduction

The Fibonacci series is a sequence of numbers in which each number is the sum of the two preceding ones, usually starting with 0 and 1. This program allows the user to input a positive integer and generates the corresponding Fibonacci sequence.

## Prerequisites

- Python 3.x

## Usage

1. Clone the repository or download the `index.py` file.
2. Ensure you have Python 3.x installed on your machine.
3. Run the program by executing the following command in your terminal:

    ```bash
    python index.py
    ```

4. Enter a positive integer when prompted.
5. The program will output the Fibonacci sequence up to the entered number.

## Code Explanation

Here's a brief explanation of the code:

```python
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n - 2) + fibonacci(n - 1)

numero = int(input("Enter a positive integer number: "))

if numero < 0:
    print("Invalid number")
else:
    print("Fibonacci sequence: ")
    for i in range(numero):
        print(fibonacci(i))
