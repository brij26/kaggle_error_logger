# Kaggle Error Logger

A simple utility to log **unhandled exceptions** in **Kaggle notebooks** (and other Python environments).

## Installation

Install the package using pip:

```python
!pip install kagglog==0.2.1

```

## How it Works

Import the library:

```python
import kagglog

```

By default, `kagglog` provides a simple way to capture errors.

If you want to log errors for a specific code block, you must call:

```python
kagglog.enable()

```

**Place `kagglog.enable()` before every code block where you want error logging to be active.**

## Example

```python
import kagglog

kagglog.enable()  # enable error logging for this block

# Example code that will raise an unhandled exception
arr = [1, 2, 3]
print(arr[5])  # This will be logged as an error (IndexError)

```

## Features

- Simple error logging for Kaggle notebooks. 📓

- Works in any Python environment.

- Minimal setup required (`import kagglog` + `kagglog.enable()`).

- Lightweight and easy to use.
