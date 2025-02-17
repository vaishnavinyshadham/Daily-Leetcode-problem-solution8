# Daily-Leetcode-problem-solution8

PROBLEM

You have n  tiles, where each tile has one letter tiles[i] printed on it.
Return the number of possible non-empty sequences of letters you can make using the letters printed on those tiles.

Intuition

solve this problem using backtracking with a frequency map to generate all possible sequences of letters.

Approach

Use a frequency map (array of size 26) to keep track of the occurrences of each letter in tiles.
Use backtracking to recursively generate all possible sequences.
At each step, iterate through all letters in the frequency map:
If the count of a letter is greater than 0, include it in the current sequence and decrement its count.
Recursively call the function to continue forming sequences.
Backtrack by restoring the count.
Keep track of the number of sequences generated.

Complexity

Time complexity:
O(k!), where k is the number of unique letters.

Space complexity:
O(26) or simply O(constant)
