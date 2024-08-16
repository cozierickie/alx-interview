# 0x01. Lockboxes

## Project Overview

This project is part of the ALX interview preparation curriculum. The goal is to solve the "Lockboxes" problem, where you are required to determine if all boxes can be opened based on the keys they contain.

### Problem Statement

You have `n` number of locked boxes in front of you, numbered sequentially from `0` to `n-1`. Each box may contain keys that open other boxes. The first box `boxes[0]` is unlocked by default.

- **Objective:** Write a method `canUnlockAll(boxes)` that determines if all boxes can be opened.
- **Input:** `boxes` is a list of lists, where each sublist represents the keys available in that box.
- **Output:** Return `True` if all boxes can be opened; otherwise, return `False`.

### Requirements

- The function must be defined as `def canUnlockAll(boxes):`.
- You can assume that all keys will be positive integers.
- Keys may not correspond to any box.
- The first box (index `0`) is already unlocked.
- The function should return a boolean value (`True` or `False`).

### Example

```python
#!/usr/bin/python3
canUnlockAll = __import__('0-lockboxes').canUnlockAll

boxes = [[1], [2], [3], [4], []]
print(canUnlockAll(boxes))  # True

boxes = [[1, 4, 6], [2], [0, 4, 1], [5, 6, 2], [3], [4, 1], [6]]
print(canUnlockAll(boxes))  # True

boxes = [[1, 4], [2], [0, 4, 1], [3], [], [4, 1], [5, 6]]
print(canUnlockAll(boxes))  # False

### How to Run
Clone the repository:
git clone https://github.com/your_username/alx-interview.git

Navigate to the project directory:
cd alx-interview/0x01-lockboxes

Make the test script executable:
chmod +x main_0.py

Run the test script:
./main_0.py
