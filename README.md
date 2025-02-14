# Hash Table Practice (JavaScript)

See the [Ruby version](https://github.com/AdaGold/hash-practice) for details.

## Installation

This has been tested with node `12.6.0`. To install, run

```
npm i
```

after cloning this project.

## Testing
Run all tests with:

```
npm test
```

Feel free to add additional tests and point out if you think they should be in the final project submission.


# Hash Table Practice

In this exercise you will complete two coding problems using Hash Tables.

## Learning Goals

By the end of this exercise you should be able to:

- Use a hash table to solve a coding problem
- Identify how a hash table can produce a more attractive runtime over alternative solutions

## Grouped Anagrams

Given an array of strings, group anagrams together.

### Example

```
Input: ["eat", "tea", "tan", "ate", "nat", "bat"],
Output:
[
  ["ate","eat","tea"],
  ["nat","tan"],
  ["bat"]
]
```

Note:

- All inputs will be in lowercase.
- The order of your output does not matter

## Most Frequent K Elements

Given a non-empty array of integers, return the *k* most frequent elements.

## Example 1

```
Input: nums = [1,1,1,2,2,3], k = 2
Output: [1,2]
```

## Example 2

```
Input: nums = [1], k = 1
Output: [1]
```

## Note

You may assume k is always valid, 1 ≤ k ≤ number of unique elements.

You should be able to equal or beat O(n log n), where n is the array's size.


## Optional: Valid Sudoku

Determine if a 9x9 Sudoku board is valid. Only the filled cells need to be validated according to the following rules:

1. Each row must contain the digits 1-9 without repetition.
1. Each column must contain the digits 1-9 without repetition.
1. Each of the 9 3x3 sub-boxes of the grid must contain the digits 1-9 without repetition.

![sudoku image](images/250px-Sudoku-by-L2G-20050714.svg.png)

Above is a valid Sudoku grid.

The Sudoku board could be partially filled, where empty cells are filled with the character '.'.

**Example 1:**

```
Input:
[
  ["5","3",".",".","7",".",".",".","."],
  ["6",".",".","1","9","5",".",".","."],
  [".","9","8",".",".",".",".","6","."],
  ["8",".",".",".","6",".",".",".","3"],
  ["4",".",".","8",".","3",".",".","1"],
  ["7",".",".",".","2",".",".",".","6"],
  [".","6",".",".",".",".","2","8","."],
  [".",".",".","4","1","9",".",".","5"],
  [".",".",".",".","8",".",".","7","9"]
]
Output: true
```


**Example 2:**

```
Input:
[
  ["8","3",".",".","7",".",".",".","."],
  ["6",".",".","1","9","5",".",".","."],
  [".","9","8",".",".",".",".","6","."],
  ["8",".",".",".","6",".",".",".","3"],
  ["4",".",".","8",".","3",".",".","1"],
  ["7",".",".",".","2",".",".",".","6"],
  [".","6",".",".",".",".","2","8","."],
  [".",".",".","4","1","9",".",".","5"],
  [".",".",".",".","8",".",".","7","9"]
]
Output: false
Explanation: Same as Example 1, except with the 5 in the top left corner being 
    modified to 8. Since there are two 8's in the top left 3x3 sub-box, it is invalid.
```