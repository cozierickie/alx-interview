# 0x04. UTF-8 Validation

## Description
This project involves validating if a dataset of integers represents valid UTF-8 encoded data. Each integer in the list represents one byte, and the goal is to ensure that the dataset conforms to the UTF-8 encoding rules.

## Learning Objectives
- Understand the UTF-8 encoding scheme and its multi-byte character structure.
- Apply bitwise operations to parse and validate byte sequences.
- Gain experience with data validation and logical operations in Python.

## Requirements
- Python 3.4.3 or higher on Ubuntu 20.04 LTS.
- Code should follow PEP 8 styling guidelines.

## Usage
The project provides a function `validUTF8(data)` that takes a list of integers and returns `True` if the data is valid UTF-8 encoding, otherwise `False`.

### Example
```python
# Import the function
from 0-validate_utf8 import validUTF8

data1 = [65]
print(validUTF8(data1))  # Output: True

data2 = [229, 65, 127, 256]
print(validUTF8(data2))  # Output: False

### Files
0-validate_utf8.py: Contains the main validation function.
0-main.py: Example test file to demonstrate functionality.
How it Works
The function uses bitwise operations to:

Identify the number of bytes a character spans based on its leading byte.
Validate that continuation bytes begin with 10.
Return True if all bytes follow valid UTF-8 encoding rules, otherwise False.
