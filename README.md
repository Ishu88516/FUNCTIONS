# Python Functions, Iterators, Generators & Functional Programming

## 📌 Overview

This project contains solutions to **theory and practical questions** based on Python functions, iterators, generators, lambda expressions, and functional programming concepts such as `map()`, `filter()`, and `reduce()`.

All programs are written in **simple, readable Python code** and are suitable for **beginners and academic assignments**.

---

## 🛠️ Technologies Used

* Python 3.x
* Google Colab / Jupyter Notebook

---

## 📂 Contents

### 🔹 Functions

* Sum of even numbers in a list
* Reverse a string
* Square of numbers in a list
* Prime number checker

### 🔹 Iterators & Generators

* Fibonacci sequence using an iterator class
* Generator for powers of 2
* Generator to read files line by line

### 🔹 Lambda & Functional Programming

* Sorting tuples using lambda
* Celsius to Fahrenheit conversion using `map()`
* Removing vowels using `filter()`
* Book shop accounting program using `lambda` and `map()`

---

## 🧪 Example Programs

### Sum of Even Numbers

```python
def sum_even_numbers(lst):
    return sum(num for num in lst if num % 2 == 0)
```

### Fibonacci Iterator

```python
class Fibonacci:
    def __init__(self, terms):
        self.terms = terms
        self.a, self.b = 0, 1
        self.count = 0

    def __iter__(self):
        return self

    def __next__(self):
        if self.count >= self.terms:
            raise StopIteration
        self.count += 1
        value = self.a
        self.a, self.b = self.b, self.a + self.b
        return value
```

---

## 📘 Assignment Coverage

✔ Functions and return values
✔ Iterators vs Iterables
✔ Generators and `yield`
✔ Lambda functions
✔ `map()`, `filter()`, `reduce()`
✔ Real-world example (Book shop accounting)

---

## ▶️ How to Run

1. Open the notebook in **Google Colab** or **Jupyter Notebook**
2. Run each cell sequentially
3. Modify input values to test different cases

