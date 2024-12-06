0x09. Island Perimeter
Description
Calculate the perimeter of an island in a 2D grid using Python. Land is represented by 1, and water is 0. The function will determine the perimeter based on land cells and their adjacency.

Task
Function: def island_perimeter(grid):

Input: 2D list of integers (0 for water, 1 for land).
Output: Perimeter of the island as an integer.
Constraints: Grid is rectangular, at most 100x100, and surrounded by water with no lakes.

Example:
grid = [
    [0, 0, 0, 0, 0, 0],
    [0, 1, 0, 0, 0, 0],
    [0, 1, 0, 0, 0, 0],
    [0, 1, 1, 1, 0, 0],
    [0, 0, 0, 0, 0, 0]
]
print(island_perimeter(grid))  # Output: 12
