
# Dynamic Programming

Sorted by frequency, only includes green and yellow.

## 5. Longest Palindromic Substring

Given a string s, find the longest palindromic substring in s. You may assume that the maximum length of s is 1000.

Example 1:
```
Input: "babad"
Output: "bab"
Note: "aba" is also a valid answer.
```

Example 2:
```
Input: "cbbd"
Output: "bb"
```

Solution:
```cpp
class Solution {
public:
    string longestPalindrome(string s) {
        
    }
};
```

## 53. Maximum Subarray

Given an integer array nums, find the contiguous subarray (containing at least one number) which has the largest sum and return its sum.

Example:
```
Input: [-2,1,-3,4,-1,2,1,-5,4],
Output: 6
Explanation: [4,-1,2,1] has the largest sum = 6.
```
Follow up:

If you have figured out the O(n) solution, try coding another solution using the divide and conquer approach, which is more subtle.

Solution:

```cpp
class Solution {
public:
    int maxSubArray(vector<int>& nums) {
        
    }
};
```

## 121. Best Time to Buy and Sell Stock

Say you have an array for which the ith element is the price of a given stock on day i.

If you were only permitted to complete at most one transaction (i.e., buy one and sell one share of the stock), design an algorithm to find the maximum profit.

Note that you cannot sell a stock before you buy one.

Example 1:
```
Input: [7,1,5,3,6,4]
Output: 5
Explanation: Buy on day 2 (price = 1) and sell on day 5 (price = 6), profit = 6-1 = 5.
             Not 7-1 = 6, as selling price needs to be larger than buying price.
```

Example 2:
```
Input: [7,6,4,3,1]
Output: 0
Explanation: In this case, no transaction is done, i.e. max profit = 0.
```

Solution:
```cpp
class Solution {
public:
    int maxProfit(vector<int>& prices) {
        
    }
};
```

## 85. Maximal Rectangle

Given a 2D binary matrix filled with 0's and 1's, find the largest rectangle containing only 1's and return its area.

Example:
```
Input:
[
  ["1","0","1","0","0"],
  ["1","0","1","1","1"],
  ["1","1","1","1","1"],
  ["1","0","0","1","0"]
]
Output: 6
```

Solution:
```cpp
class Solution {
public:
    int maximalRectangle(vector<vector<char>>& matrix) {
        
    }
};
```

## 10. Regular Expression Matching

Given an input string (s) and a pattern (p), implement regular expression matching with support for '.' and '*'.
```
'.' Matches any single character.
'*' Matches zero or more of the preceding element.
```
The matching should cover the entire input string (not partial).

Note:

- s could be empty and contains only lowercase letters a-z.
- p could be empty and contains only lowercase letters a-z, and characters like . or *.

Example 1:
```
Input:
s = "aa"
p = "a"
Output: false
Explanation: "a" does not match the entire string "aa".
```
Example 2:
```
Input:
s = "aa"
p = "a*"
Output: true
Explanation: '*' means zero or more of the preceding element, 'a'. 
Therefore, by repeating 'a' once, it becomes "aa".
```
Example 3:
```
Input:
s = "ab"
p = ".*"
Output: true
Explanation: ".*" means "zero or more (*) of any character (.)".
```
Example 4:
```
Input:
s = "aab"
p = "c*a*b"
Output: true
Explanation: c can be repeated 0 times, a can be repeated 1 time. 
Therefore, it matches "aab".
```

Example 5:
```
Input:
s = "mississippi"
p = "mis*is*p*."
Output: false
```

Solution:
```cpp
class Solution {
public:
    bool isMatch(string s, string p) {
        
    }
};
```

## 312. Burst Balloons

Given n balloons, indexed from 0 to n-1. Each balloon is painted with a number on it represented by array nums. You are asked to burst all the balloons. If the you burst balloon i you will get nums[left] * nums[i] * nums[right] coins. Here left and right are adjacent indices of i. After the burst, the left and right then becomes adjacent.

Find the maximum coins you can collect by bursting the balloons wisely.

Note:

- You may imagine nums[-1] = nums[n] = 1. They are not real therefore you can not burst them.
- 0 ≤ n ≤ 500, 0 ≤ nums[i] ≤ 100

Example:

```
Input: [3,1,5,8]
Output: 167 
Explanation: nums = [3,1,5,8] --> [3,5,8] -->   [3,8]   -->  [8]  --> []
             coins =  3*1*5      +  3*5*8    +  1*3*8      + 1*8*1   = 167
```

Solution:
```cpp
class Solution {
public:
    int maxCoins(vector<int>& nums) {
        
    }
};
```

## 96. Unique Binary Search Trees

Given n, how many structurally unique BST's (binary search trees) that store values 1 ... n?

Example:
```
Input: 3
Output: 5
Explanation:
Given n = 3, there are a total of 5 unique BST's:

   1         3     3      2      1
    \       /     /      / \      \
     3     2     1      1   3      2
    /     /       \                 \
   2     1         2                 3
```

Solution:
```cpp
class Solution {
public:
    int numTrees(int n) {
        
    }
};
```

## 70. Climbing Stairs

You are climbing a stair case. It takes n steps to reach to the top.

Each time you can either climb 1 or 2 steps. In how many distinct ways can you climb to the top?

Example 1:
```
Input: 2
Output: 2
Explanation: There are two ways to climb to the top.
1. 1 step + 1 step
2. 2 steps
```
Example 2:
```
Input: 3
Output: 3
Explanation: There are three ways to climb to the top.
1. 1 step + 1 step + 1 step
2. 1 step + 2 steps
3. 2 steps + 1 step
```

Constraints:

- 1 <= n <= 45

Solution:
```cpp
class Solution {
public:
    int climbStairs(int n) {
        
    }
};
```

## 198. House Robber

You are a professional robber planning to rob houses along a street. Each house has a certain amount of money stashed, the only constraint stopping you from robbing each of them is that adjacent houses have security system connected and it will automatically contact the police if two adjacent houses were broken into on the same night.

Given a list of non-negative integers representing the amount of money of each house, determine the maximum amount of money you can rob tonight without alerting the police.

 

Example 1:
```
Input: nums = [1,2,3,1]
Output: 4
Explanation: Rob house 1 (money = 1) and then rob house 3 (money = 3).
             Total amount you can rob = 1 + 3 = 4.
```
Example 2:
```
Input: nums = [2,7,9,3,1]
Output: 12
Explanation: Rob house 1 (money = 2), rob house 3 (money = 9) and rob house 5 (money = 1).
             Total amount you can rob = 2 + 9 + 1 = 12.
```

Constraints:

- 0 <= nums.length <= 100
- 0 <= nums[i] <= 400

Solution:
```cpp
class Solution {
public:
    int rob(vector<int>& nums) {
        
    }
};
```

## 139. Word Break

Given a non-empty string s and a dictionary wordDict containing a list of non-empty words, determine if s can be segmented into a space-separated sequence of one or more dictionary words.

Note:

The same word in the dictionary may be reused multiple times in the segmentation.
You may assume the dictionary does not contain duplicate words.

Example 1:
```
Input: s = "leetcode", wordDict = ["leet", "code"]
Output: true
Explanation: Return true because "leetcode" can be segmented as "leet code".
```
Example 2:
```
Input: s = "applepenapple", wordDict = ["apple", "pen"]
Output: true
Explanation: Return true because "applepenapple" can be segmented as "apple pen apple".
             Note that you are allowed to reuse a dictionary word.
```             
Example 3:
```
Input: s = "catsandog", wordDict = ["cats", "dog", "sand", "and", "cat"]
Output: false
```

Solution:
```cpp
class Solution {
public:
    bool wordBreak(string s, vector<string>& wordDict) {
        
    }
};
```

## 72. Edit Distance

Given two words word1 and word2, find the minimum number of operations required to convert word1 to word2.

You have the following 3 operations permitted on a word:

Insert a character
Delete a character
Replace a character

Example 1:
```
Input: word1 = "horse", word2 = "ros"
Output: 3
Explanation: 
horse -> rorse (replace 'h' with 'r')
rorse -> rose (remove 'r')
rose -> ros (remove 'e')
```
Example 2:
```
Input: word1 = "intention", word2 = "execution"
Output: 5
Explanation: 
intention -> inention (remove 't')
inention -> enention (replace 'i' with 'e')
enention -> exention (replace 'n' with 'x')
exention -> exection (replace 'n' with 'c')
exection -> execution (insert 'u')
```
Solution:
```cpp
class Solution {
public:
    int minDistance(string word1, string word2) {
        
    }
};
```

## 152. Maximum Product Subarray

Given an integer array nums, find the contiguous subarray within an array (containing at least one number) which has the largest product.

Example 1:
```
Input: [2,3,-2,4]
Output: 6
Explanation: [2,3] has the largest product 6.
```
Example 2:
```
Input: [-2,0,-1]
Output: 0
Explanation: The result cannot be 2, because [-2,-1] is not a subarray.
```

Solution:
```cpp
class Solution {
public:
    int maxProduct(vector<int>& nums) {
        
    }
};
```

## 1130. Minimum Cost Tree From Leaf Values

Given an array arr of positive integers, consider all binary trees such that:

- Each node has either 0 or 2 children;
- The values of arr correspond to the values of each leaf in an in-order traversal of the tree.  (Recall that a node is a leaf if and only if it has 0 children.)
- The value of each non-leaf node is equal to the product of the largest leaf value in its left and right subtree respectively.

Among all possible binary trees considered, return the smallest possible sum of the values of each non-leaf node.  It is guaranteed this sum fits into a 32-bit integer. 

Example 1:
```
Input: arr = [6,2,4]
Output: 32
Explanation:
There are two possible trees.  The first has non-leaf node sum 36, and the 
second has non-leaf node sum 32.

    24            24
   /  \          /  \
  12   4        6    8
 /  \               / \
6    2             2   4
```

Constraints:

- 2 <= arr.length <= 40
- 1 <= arr[i] <= 15
- It is guaranteed that the answer fits into a 32-bit signed integer (ie. it is less than 2^31).

Solution:
```cpp
class Solution {
public:
    int mctFromLeafValues(vector<int>& arr) {
        
    }
};
```

## 338. Counting Bits

Given a non negative integer number num. For every numbers i in the range 0 ≤ i ≤ num calculate the number of 1's in their binary representation and return them as an array.

Example 1:
```
Input: 2
Output: [0,1,1]
```
Example 2:
```
Input: 5
Output: [0,1,1,2,1,2]
```
Follow up:

- It is very easy to come up with a solution with run time O(n*sizeof(integer)). But can you do it in linear time O(n) /possibly in a single pass?
- Space complexity should be O(n).
- Can you do it like a boss? Do it without using any builtin function like __builtin_popcount in c++ or in any other language.

Solution:
```cpp
class Solution {
public:
    vector<int> countBits(int num) {
        
    }
};
```

## 279. Perfect Squares

Given a positive integer n, find the least number of perfect square numbers (for example, 1, 4, 9, 16, ...) which sum to n.

Example 1:
```
Input: n = 12
Output: 3 
Explanation: 12 = 4 + 4 + 4.
```
Example 2:
```
Input: n = 13
Output: 2
Explanation: 13 = 4 + 9.
```

Solution:
```cpp
class Solution {
public:
    int numSquares(int n) {
        
    }
};
```

## 120. Triangle

Given a triangle, find the minimum path sum from top to bottom. Each step you may move to adjacent numbers on the row below.

For example, given the following triangle
```
[
     [2],
    [3,4],
   [6,5,7],
  [4,1,8,3]
]
```
The minimum path sum from top to bottom is 11 (i.e., 2 + 3 + 5 + 1 = 11).

Note:

Bonus point if you are able to do this using only O(n) extra space, where n is the total number of rows in the triangle.

Solution:
```cpp
class Solution {
public:
    int minimumTotal(vector<vector<int>>& triangle) {
        
    }
};
```

## 64. Minimum Path Sum

Given a m x n grid filled with non-negative numbers, find a path from top left to bottom right which minimizes the sum of all numbers along its path.

Note: You can only move either down or right at any point in time.

Example:
```
Input:
[
  [1,3,1],
  [1,5,1],
  [4,2,1]
]
Output: 7
Explanation: Because the path 1→3→1→1→1 minimizes the sum.
```

Solution:
```cpp
class Solution {
public:
    int minPathSum(vector<vector<int>>& grid) {
        
    }
};
```

## 309. Best Time to Buy and Sell Stock with Cooldown

Say you have an array for which the ith element is the price of a given stock on day i.

Design an algorithm to find the maximum profit. You may complete as many transactions as you like (ie, buy one and sell one share of the stock multiple times) with the following restrictions:

- You may not engage in multiple transactions at the same time (ie, you must sell the stock before you buy again).
- After you sell your stock, you cannot buy stock on next day. (ie, cooldown 1 day)

Example:
```
Input: [1,2,3,0,2]
Output: 3 
Explanation: transactions = [buy, sell, cooldown, buy, sell]
```

Solution:
```cpp
class Solution {
public:
    int maxProfit(vector<int>& prices) {
        
    }
};
```

## 1025. Divisor Game

Alice and Bob take turns playing a game, with Alice starting first.

Initially, there is a number N on the chalkboard.  On each player's turn, that player makes a move consisting of:

Choosing any x with 0 < x < N and N % x == 0.
Replacing the number N on the chalkboard with N - x.
Also, if a player cannot make a move, they lose the game.

Return True if and only if Alice wins the game, assuming both players play optimally.

Example 1:
```
Input: 2
Output: true
Explanation: Alice chooses 1, and Bob has no more moves.
```
Example 2:
```
Input: 3
Output: false
Explanation: Alice chooses 1, Bob chooses 1, and Alice has no more moves.
```

Note:

- 1 <= N <= 1000

Solution:
```cpp
class Solution {
public:
    bool divisorGame(int N) {
        
    }
};
```

## 32. Longest Valid Parentheses

Given a string containing just the characters '(' and ')', find the length of the longest valid (well-formed) parentheses substring.

Example 1:
```
Input: "(()"
Output: 2
Explanation: The longest valid parentheses substring is "()"
```
Example 2:
```
Input: ")()())"
Output: 4
Explanation: The longest valid parentheses substring is "()()"
```

Solution:
```cpp
class Solution {
public:
    int longestValidParentheses(string s) {
        
    }
};
```

## 95. Unique Binary Search Trees II

Given an integer n, generate all structurally unique BST's (binary search trees) that store values 1 ... n.

Example:
```
Input: 3
Output:
[
  [1,null,3,2],
  [3,2,null,1],
  [3,1,null,null,2],
  [2,1,3],
  [1,null,2,null,3]
]
Explanation:
The above output corresponds to the 5 unique BST's shown below:

   1         3     3      2      1
    \       /     /      / \      \
     3     2     1      1   3      2
    /     /       \                 \
   2     1         2                 3
```

Constraints:

- 0 <= n <= 8

Solution:
```cpp
/**
 * Definition for a binary tree node.
 * struct TreeNode {
 *     int val;
 *     TreeNode *left;
 *     TreeNode *right;
 *     TreeNode() : val(0), left(nullptr), right(nullptr) {}
 *     TreeNode(int x) : val(x), left(nullptr), right(nullptr) {}
 *     TreeNode(int x, TreeNode *left, TreeNode *right) : val(x), left(left), right(right) {}
 * };
 */
class Solution {
public:
    vector<TreeNode*> generateTrees(int n) {
        
    }
};
```

## 357. Count Numbers with Unique Digits

Given a non-negative integer n, count all numbers with unique digits, x, where 0 ≤ x < 10n.

Example:
```
Input: 2
Output: 91 
Explanation: The answer should be the total numbers in the range of 0 ≤ x < 100, 
             excluding 11,22,33,44,55,66,77,88,99
```

Constraints:

- 0 <= n <= 8

Solution:
```cpp
class Solution {
public:
    int countNumbersWithUniqueDigits(int n) {
        
    }
};
```

## 123. Best Time to Buy and Sell Stock III

Say you have an array for which the ith element is the price of a given stock on day i.

Design an algorithm to find the maximum profit. You may complete at most two transactions.

Note: You may not engage in multiple transactions at the same time (i.e., you must sell the stock before you buy again).

Example 1:
```
Input: [3,3,5,0,0,3,1,4]
Output: 6
Explanation: Buy on day 4 (price = 0) and sell on day 6 (price = 3), 
             profit = 3-0 = 3. Then buy on day 7 (price = 1) and sell
             on day 8 (price = 4), profit = 4-1 = 3.
```
Example 2:
```            
Input: [1,2,3,4,5]
Output: 4
Explanation: Buy on day 1 (price = 1) and sell on day 5 (price = 5), 
             profit = 5-1 = 4. Note that you cannot buy on day 1, 
             buy on day 2 and sell them later, as you are
             engaging multiple transactions at the same time. 
             You must sell before buying again.
```
Example 3:
```        
Input: [7,6,4,3,1]
Output: 0
Explanation: In this case, no transaction is done, i.e. max profit = 0.
```

Solution:
```cpp
class Solution {
public:
    int maxProfit(vector<int>& prices) {
        
    }
};
```

## 62. Unique Paths

A robot is located at the top-left corner of a m x n grid (marked 'Start' in the diagram below).

The robot can only move either down or right at any point in time. The robot is trying to reach the bottom-right corner of the grid (marked 'Finish' in the diagram below).

How many possible unique paths are there?

![](https://assets.leetcode.com/uploads/2018/10/22/robot_maze.png)

Above is a 7 x 3 grid. How many possible unique paths are there?

Example 1:
```
Input: m = 3, n = 2
Output: 3
Explanation:
From the top-left corner, there are a total of 3 ways to reach the bottom-right corner:
1. Right -> Right -> Down
2. Right -> Down -> Right
3. Down -> Right -> Right
```

Example 2:
```
Input: m = 7, n = 3
Output: 28
```

Constraints:

- 1 <= m, n <= 100
- It's guaranteed that the answer will be less than or equal to 2 * 10 ^ 9.

Solution:
```cpp
class Solution {
public:
    int uniquePaths(int m, int n) {
        
    }
};
```

## 303. Range Sum Query - Immutable

Given an integer array nums, find the sum of the elements between indices i and j (i ≤ j), inclusive.

Example:
```
Given nums = [-2, 0, 3, -5, 2, -1]

sumRange(0, 2) -> 1
sumRange(2, 5) -> -1
sumRange(0, 5) -> -3
```
Note:
- You may assume that the array does not change.
- There are many calls to sumRange function.

Solution:
```cpp
class NumArray {
public:
    NumArray(vector<int>& nums) {
        
    }
    
    int sumRange(int i, int j) {
        
    }
};

/**
 * Your NumArray object will be instantiated and called as such:
 * NumArray* obj = new NumArray(nums);
 * int param_1 = obj->sumRange(i,j);
 */
```

## 413. Arithmetic Slices

A sequence of numbers is called arithmetic if it consists of at least three elements and if the difference between any two consecutive elements is the same.

For example, these are arithmetic sequences:
```
1, 3, 5, 7, 9
7, 7, 7, 7
3, -1, -5, -9
```
The following sequence is not arithmetic.
```
1, 1, 2, 5, 7
```
A zero-indexed array A consisting of N numbers is given. A slice of that array is any pair of integers (P, Q) such that 0 <= P < Q < N.

A slice (P, Q) of the array A is called arithmetic if the sequence:
A[P], A[P + 1], ..., A[Q - 1], A[Q] is arithmetic. In particular, this means that P + 1 < Q.

The function should return the number of arithmetic slices in the array A.

 
Example:
```
A = [1, 2, 3, 4]

return: 3, for 3 arithmetic slices in A: [1, 2, 3], [2, 3, 4] 
and [1, 2, 3, 4] itself.
```

Solution:
```cpp
class Solution {
public:
    int numberOfArithmeticSlices(vector<int>& A) {
        
    }
};
```

## 647. Palindromic Substrings

Given a string, your task is to count how many palindromic substrings in this string.

The substrings with different start indexes or end indexes are counted as different substrings even they consist of same characters.

Example 1:
```
Input: "abc"
Output: 3
Explanation: Three palindromic strings: "a", "b", "c".
```

Example 2:
```
Input: "aaa"
Output: 6
Explanation: Six palindromic strings: "a", "a", "a", "aa", "aa", "aaa".
```

Note:

- The input string length won't exceed 1000.

Solution:
```cpp
class Solution {
public:
    int countSubstrings(string s) {
        
    }
};
```

## 140. Word Break II

Given a non-empty string s and a dictionary wordDict containing a list of non-empty words, add spaces in s to construct a sentence where each word is a valid dictionary word. Return all such possible sentences.

Note:

- The same word in the dictionary may be reused multiple times in the segmentation.
- You may assume the dictionary does not contain duplicate words.

Example 1:
```
Input:
s = "catsanddog"
wordDict = ["cat", "cats", "and", "sand", "dog"]
Output:
[
  "cats and dog",
  "cat sand dog"
]
```
Example 2:
```
Input:
s = "pineapplepenapple"
wordDict = ["apple", "pen", "applepen", "pine", "pineapple"]
Output:
[
  "pine apple pen apple",
  "pineapple pen apple",
  "pine applepen apple"
]
Explanation: Note that you are allowed to reuse a dictionary word.
```
Example 3:
```
Input:
s = "catsandog"
wordDict = ["cats", "dog", "sand", "and", "cat"]
Output:
[]
```

Solution:
```cpp
class Solution {
public:
    vector<string> wordBreak(string s, vector<string>& wordDict) {
        
    }
};
```

## 221. Maximal Square

Given a 2D binary matrix filled with 0's and 1's, find the largest square containing only 1's and return its area.

Example:
```
Input: 

1 0 1 0 0
1 0 1 1 1
1 1 1 1 1
1 0 0 1 0

Output: 4
```

Solution:
```cpp
class Solution {
public:
    int maximalSquare(vector<vector<char>>& matrix) {
        
    }
};
```

## 91. Decode Ways

A message containing letters from A-Z is being encoded to numbers using the following mapping:
```
'A' -> 1
'B' -> 2
...
'Z' -> 26
```
Given a non-empty string containing only digits, determine the total number of ways to decode it.

Example 1:
```
Input: "12"
Output: 2
Explanation: It could be decoded as "AB" (1 2) or "L" (12).
```
Example 2:
```
Input: "226"
Output: 3
Explanation: It could be decoded as "BZ" (2 26), "VF" (22 6), or "BBF" (2 2 6).
```

Solution:
```cpp
class Solution {
public:
    int numDecodings(string s) {
        
    }
};
```

## 97. Interleaving String

Given s1, s2, s3, find whether s3 is formed by the interleaving of s1 and s2.

Example 1:
```
Input: s1 = "aabcc", s2 = "dbbca", s3 = "aadbbcbcac"
Output: true
```
Example 2:
```
Input: s1 = "aabcc", s2 = "dbbca", s3 = "aadbbbaccc"
Output: false
```

Solution:
```cpp
class Solution {
public:
    bool isInterleave(string s1, string s2, string s3) {
        
    }
};
```

## 115. Distinct Subsequences

Given a string S and a string T, count the number of distinct subsequences of S which equals T.

A subsequence of a string is a new string which is formed from the original string by deleting some (can be none) of the characters without disturbing the relative positions of the remaining characters. (ie, "ACE" is a subsequence of "ABCDE" while "AEC" is not).

It's guaranteed the answer fits on a 32-bit signed integer.

Example 1:
```
Input: S = "rabbbit", T = "rabbit"
Output: 3
Explanation:
As shown below, there are 3 ways you can generate "rabbit" from S.
(The caret symbol ^ means the chosen letters)

rabbbit
^^^^ ^^
rabbbit
^^ ^^^^
rabbbit
^^^ ^^^
```
Example 2:
```
Input: S = "babgbag", T = "bag"
Output: 5
Explanation:
As shown below, there are 5 ways you can generate "bag" from S.
(The caret symbol ^ means the chosen letters)

babgbag
^^ ^
babgbag
^^    ^
babgbag
^    ^^
babgbag
  ^  ^^
babgbag
    ^^^
```

Solution:
```cpp
class Solution {
public:
    int numDistinct(string s, string t) {
        
    }
};
```

## 1140. Stone Game II

Alex and Lee continue their games with piles of stones.  There are a number of piles arranged in a row, and each pile has a positive integer number of stones piles[i].  The objective of the game is to end with the most stones. 

Alex and Lee take turns, with Alex starting first.  Initially, M = 1.

On each player's turn, that player can take all the stones in the first X remaining piles, where 1 <= X <= 2M.  Then, we set M = max(M, X).

The game continues until all the stones have been taken.

Assuming Alex and Lee play optimally, return the maximum number of stones Alex can get.

 

Example 1:
```
Input: piles = [2,7,9,4,4]
Output: 10
Explanation:  If Alex takes one pile at the beginning, 
Lee takes two piles, then Alex takes 2 piles again. Alex 
can get 2 + 4 + 4 = 10 piles in total. If Alex takes two 
piles at the beginning, then Lee can take all three piles 
left. In this case, Alex get 2 + 7 = 9 piles in total. So 
we return 10 since it's larger. 
``` 

Constraints:

- 1 <= piles.length <= 100
- 1 <= piles[i] <= 10 ^ 4

Solution:
```cpp
class Solution {
public:
    int stoneGameII(vector<int>& piles) {
        
    }
};
```

## 322. Coin Change

You are given coins of different denominations and a total amount of money amount. Write a function to compute the fewest number of coins that you need to make up that amount. If that amount of money cannot be made up by any combination of the coins, return -1.

Example 1:

```
Input: coins = [1, 2, 5], amount = 11
Output: 3 
Explanation: 11 = 5 + 5 + 1
```
Example 2:
```
Input: coins = [2], amount = 3
Output: -1
```
Note:
You may assume that you have an infinite number of each kind of coin.

Solution:
```cpp
class Solution {
public:
    int coinChange(vector<int>& coins, int amount) {
        
    }
};
```

## 410. Split Array Largest Sum
 
Given an array which consists of non-negative integers and an integer m, you can split the array into m non-empty continuous subarrays. Write an algorithm to minimize the largest sum among these m subarrays.

Note:
If n is the length of array, assume the following constraints are satisfied:

- 1 ≤ n ≤ 1000
- 1 ≤ m ≤ min(50, n)

Examples:
```            
Input:
nums = [7,2,5,10,8]
m = 2

Output:
18

Explanation:
There are four ways to split nums into two subarrays.
The best way is to split it into [7,2,5] and [10,8],
where the largest sum among the two subarrays is only 18.
```

```cpp
class Solution {
public:
    int splitArray(vector<int>& nums, int m) {
        
    }
};
```

## 375. Guess Number Higher or Lower II

We are playing the Guess Game. The game is as follows:

I pick a number from 1 to n. You have to guess which number I picked.

Every time you guess wrong, I'll tell you whether the number I picked is higher or lower.

However, when you guess a particular number x, and you guess wrong, you pay $x. You win the game when you guess the number I picked.

Example:
```
n = 10, I pick 8.

First round:  You guess 5, I tell you that it's higher. You pay $5.
Second round: You guess 7, I tell you that it's higher. You pay $7.
Third round:  You guess 9, I tell you that it's lower. You pay $9.

Game over. 8 is the number I picked.

You end up paying $5 + $7 + $9 = $21.
```

Given a particular n ≥ 1, find out how much money you need to have to guarantee a win.

Solution:
```cpp
class Solution {
public:
    int getMoneyAmount(int n) {
        
    }
};
```

## 188. Best Time to Buy and Sell Stock IV

Say you have an array for which the i-th element is the price of a given stock on day i.

Design an algorithm to find the maximum profit. You may complete at most k transactions.

Note:
You may not engage in multiple transactions at the same time (ie, you must sell the stock before you buy again).

Example 1:
```
Input: [2,4,1], k = 2
Output: 2
Explanation: Buy on day 1 (price = 2) and sell on day 2 (price = 4), 
profit = 4-2 = 2.
```
Example 2:
```
Input: [3,2,6,5,0,3], k = 2
Output: 7
Explanation: Buy on day 2 (price = 2) and sell on day 3 (price = 6), 
             profit = 6-2 = 4. Then buy on day 5 (price = 0) and sell 
             on day 6 (price = 3), profit = 3-0 = 3.
```

Solution:
```cpp
class Solution {
public:
    int maxProfit(int k, vector<int>& prices) {
        
    }
};
```

## 87. Scramble String

Given a string s1, we may represent it as a binary tree by partitioning it to two non-empty substrings recursively.

Below is one possible representation of s1 = "great":
```
    great
   /    \
  gr    eat
 / \    /  \
g   r  e   at
           / \
          a   t
```          
To scramble the string, we may choose any non-leaf node and swap its two children.

For example, if we choose the node "gr" and swap its two children, it produces a scrambled string "rgeat".
```
    rgeat
   /    \
  rg    eat
 / \    /  \
r   g  e   at
           / \
          a   t
```          
We say that "rgeat" is a scrambled string of "great".

Similarly, if we continue to swap the children of nodes "eat" and "at", it produces a scrambled string "rgtae".
```
    rgtae
   /    \
  rg    tae
 / \    /  \
r   g  ta  e
       / \
      t   a
```      
We say that "rgtae" is a scrambled string of "great".

Given two strings s1 and s2 of the same length, determine if s2 is a scrambled string of s1.

Example 1:
```
Input: s1 = "great", s2 = "rgeat"
Output: true
```
Example 2:
```
Input: s1 = "abcde", s2 = "caebd"
Output: false
```

Solution:
```cpp
class Solution {
public:
    bool isScramble(string s1, string s2) {
        
    }
};
```

## 343. Integer Break

Given a positive integer n, break it into the sum of at least two positive integers and maximize the product of those integers. Return the maximum product you can get.

Example 1:
```
Input: 2
Output: 1
Explanation: 2 = 1 + 1, 1 × 1 = 1.
```
Example 2:
```
Input: 10
Output: 36
Explanation: 10 = 3 + 3 + 4, 3 × 3 × 4 = 36.
```
Note: You may assume that n is not less than 2 and not larger than 58.

Solution:
```cpp
class Solution {
public:
    int integerBreak(int n) {
        
    }
};
```

## 1240. Tiling a Rectangle with the Fewest Squares

Given a rectangle of size n x m, find the minimum number of integer-sided squares that tile the rectangle.

Example 1:

![](https://assets.leetcode.com/uploads/2019/10/17/sample_11_1592.png)
```
Input: n = 2, m = 3
Output: 3
Explanation: 3 squares are necessary to cover the rectangle.
2 (squares of 1x1)
1 (square of 2x2)
```
Example 2:

![](https://assets.leetcode.com/uploads/2019/10/17/sample_22_1592.png)
```
Input: n = 5, m = 8
Output: 5
```

Example 3:

![](https://assets.leetcode.com/uploads/2019/10/17/sample_33_1592.png)

```
Input: n = 11, m = 13
Output: 6
``` 

Constraints:

- 1 <= n <= 13
- 1 <= m <= 13

Solution:
```cpp
class Solution {
public:
    int tilingRectangle(int n, int m) {
        
    }
};
```

## 264. Ugly Number II

Write a program to find the n-th ugly number.

Ugly numbers are positive numbers whose prime factors only include 2, 3, 5. 

Example:
```
Input: n = 10
Output: 12
Explanation: 1, 2, 3, 4, 5, 6, 8, 9, 10, 12 is the sequence of the first 10 ugly numbers.
```
Note:  

- 1 is typically treated as an ugly number.
- n does not exceed 1690.

Solution:
```cpp
class Solution {
public:
    int nthUglyNumber(int n) {
        
    }
};
```

## 546. Remove Boxes

Given several boxes with different colors represented by different positive numbers.
You may experience several rounds to remove boxes until there is no box left. Each time you can choose some continuous boxes with the same color (composed of k boxes, k >= 1), remove them and get k*k points.
Find the maximum points you can get.

Example 1:
```
Input: boxes = [1,3,2,2,2,3,4,3,1]
Output: 23
Explanation:
[1, 3, 2, 2, 2, 3, 4, 3, 1] 
----> [1, 3, 3, 4, 3, 1] (3*3=9 points) 
----> [1, 3, 3, 3, 1] (1*1=1 points) 
----> [1, 1] (3*3=9 points) 
----> [] (2*2=4 points)
```

Constraints:

- 1 <= boxes.length <= 100
- 1 <= boxes[i] <= 100

Solution:
```cpp
class Solution {
public:
    int removeBoxes(vector<int>& boxes) {
        
    }
};
```

## 300. Longest Increasing Subsequence

Given an unsorted array of integers, find the length of longest increasing subsequence.

Example:
```
Input: [10,9,2,5,3,7,101,18]
Output: 4 
Explanation: The longest increasing subsequence is [2,3,7,101], 
therefore the length is 4. 
```
Note:

- There may be more than one LIS combination, it is only necessary for you to return the length.
- Your algorithm should run in O(n2) complexity.

Follow up: Could you improve it to O(n log n) time complexity?

Solution:
```cpp
class Solution {
public:
    int lengthOfLIS(vector<int>& nums) {
        
    }
};
```

## 363. Max Sum of Rectangle No Larger Than K

Given a non-empty 2D matrix matrix and an integer k, find the max sum of a rectangle in the matrix such that its sum is no larger than k.

Example:
```
Input: matrix = [[1,0,1],[0,-2,3]], k = 2
Output: 2 
Explanation: Because the sum of rectangle [[0, 1], [-2, 3]] is 2,
             and 2 is the max number no larger than k (k = 2).
```             
Note:

- The rectangle inside the matrix must have an area > 0.
- What if the number of rows is much larger than the number of columns?

Solution:
```cpp
class Solution {
public:
    int maxSumSubmatrix(vector<vector<int>>& matrix, int k) {
        
    }
};
```

## 730. Count Different Palindromic Subsequences

Given a string S, find the number of different non-empty palindromic subsequences in S, and return that number modulo 10^9 + 7.

A subsequence of a string S is obtained by deleting 0 or more characters from S.

A sequence is palindromic if it is equal to the sequence reversed.

Two sequences A_1, A_2, ... and B_1, B_2, ... are different if there is some i for which A_i != B_i.

Example 1:
```
Input: 
S = 'bccb'
Output: 6
Explanation: 
The 6 different non-empty palindromic subsequences
are 'b', 'c', 'bb', 'cc', 'bcb', 'bccb'.

Note that 'bcb' is counted only once, even though 
it occurs twice.
```

Example 2:
```
Input: 
S = 

'abcdabcdabcdabcdabcdabcdabcdabcddcbadcbadcbadcbadcbadcbadcbadcba'

Output: 104860361
Explanation: 
There are 3104860382 different non-empty palindromic subsequences, 
which is 104860361 modulo 10^9 + 7.
```
Note:

- The length of S will be in the range [1, 1000].
- Each character S[i] will be in the set {'a', 'b', 'c', 'd'}.

Solution:
```cpp
class Solution {
public:
    int countPalindromicSubsequences(string S) {
        
    }
};
```

## 698. Partition to K Equal Sum Subsets

Given an array of integers nums and a positive integer k, find whether it's possible to divide this array into k non-empty subsets whose sums are all equal.

Example 1:
```
Input: nums = [4, 3, 2, 3, 5, 2, 1], k = 4
Output: True
Explanation: It's possible to divide it into 4 subsets (5), 
(1, 4), (2,3), (2,3) with equal sums.
``` 

Note:

- 1 <= k <= len(nums) <= 16.
- 0 < nums[i] < 10000.

Solution:
```cpp
class Solution {
public:
    bool canPartitionKSubsets(vector<int>& nums, int k) {
        
    }
};
```

## 877. Stone Game

Alex and Lee play a game with piles of stones.  There are an even number of piles arranged in a row, and each pile has a positive integer number of stones piles[i].

The objective of the game is to end with the most stones.  The total number of stones is odd, so there are no ties.

Alex and Lee take turns, with Alex starting first.  Each turn, a player takes the entire pile of stones from either the beginning or the end of the row.  This continues until there are no more piles left, at which point the person with the most stones wins.

Assuming Alex and Lee play optimally, return True if and only if Alex wins the game.

 

Example 1:
```
Input: [5,3,4,5]
Output: true
Explanation: 
Alex starts first, and can only take the first 5 or the last 5.
Say he takes the first 5, so that the row becomes [3, 4, 5].
If Lee takes 3, then the board is [4, 5], and Alex takes 5 to win with 10 points.
If Lee takes the last 5, then the board is [3, 4], and Alex takes 4 to win with 9 points.
This demonstrated that taking the first 5 was a winning move for Alex, so we return true.
```

Note:

- 2 <= piles.length <= 500
- piles.length is even.
- 1 <= piles[i] <= 500
- sum(piles) is odd.

Solution:
```cpp
class Solution {
public:
    bool stoneGame(vector<int>& piles) {
        
    }
};
```

## 746. Min Cost Climbing Stairs

On a staircase, the i-th step has some non-negative cost cost[i] assigned (0 indexed).

Once you pay the cost, you can either climb one or two steps. You need to find minimum cost to reach the top of the floor, and you can either start from the step with index 0, or the step with index 1.

Example 1:
```
Input: cost = [10, 15, 20]
Output: 15
Explanation: Cheapest is start on cost[1], pay that cost and go to the top.
```
Example 2:
```
Input: cost = [1, 100, 1, 1, 1, 100, 1, 1, 100, 1]
Output: 6
Explanation: Cheapest is start on cost[0], and only step on 1s, skipping cost[3].
```
Note:
- cost will have a length in the range [2, 1000].
- Every cost[i] will be an integer in the range [0, 999].

Solution:
```cpp
class Solution {
public:
    int minCostClimbingStairs(vector<int>& cost) {
        
    }
};
```

## 741. Cherry Pickup

In a N x N grid representing a field of cherries, each cell is one of three possible integers.

- 0 means the cell is empty, so you can pass through;
- 1 means the cell contains a cherry, that you can pick up and pass through;
- -1 means the cell contains a thorn that blocks your way.
 
Your task is to collect maximum number of cherries possible by following the rules below:

- Starting at the position (0, 0) and reaching (N-1, N-1) by moving right or down through valid path cells (cells with value 0 or 1);
- After reaching (N-1, N-1), returning to (0, 0) by moving left or up through valid path cells;
- When passing through a path cell containing a cherry, you pick it up and the cell becomes an empty cell (0);
- If there is no valid path between (0, 0) and (N-1, N-1), then no cherries can be collected.
 
Example 1:
```
Input: grid =
[[0, 1, -1],
 [1, 0, -1],
 [1, 1,  1]]
Output: 5

Explanation: 
The player started at (0, 0) and went down, down, right right 
to reach (2, 2).
4 cherries were picked up during this single trip, and the 
matrix becomes [[0,1,-1],[0,0,-1],[0,0,0]].
Then, the player went left, up, up, left to return home,
picking up one more cherry.
The total number of cherries picked up is 5, and this is 
the maximum possible.
```

Note:

- grid is an N by N 2D array, with 1 <= N <= 50.
- Each grid[i][j] is an integer in the set {-1, 0, 1}.
- It is guaranteed that grid[0][0] and grid[N-1][N-1] are not -1.
 
 Solution:
 ```cpp
 class Solution {
public:
    int cherryPickup(vector<vector<int>>& grid) {
        
    }
};
 ```
 
## 516. Longest Palindromic Subsequence

Given a string s, find the longest palindromic subsequence's length in s. You may assume that the maximum length of s is 1000.

Example 1:
```
Input:

"bbbab"
```
Output:
```
4
```
One possible longest palindromic subsequence is "bbbb".
 

Example 2:
Input:
```
"cbbd"
```
Output:
```
2
```
One possible longest palindromic subsequence is "bb".
 

Constraints:

- 1 <= s.length <= 1000
- s consists only of lowercase English letters.

Solution:
```cpp
class Solution {
public:
    int longestPalindromeSubseq(string s) {
        
    }
};
```

## 354. Russian Doll Envelopes

You have a number of envelopes with widths and heights given as a pair of integers (w, h). One envelope can fit into another if and only if both the width and height of one envelope is greater than the width and height of the other envelope.

What is the maximum number of envelopes can you Russian doll? (put one inside other)

Note:
Rotation is not allowed.

Example:
```
Input: [[5,4],[6,4],[6,7],[2,3]]
Output: 3 
Explanation: The maximum number of envelopes you can 
Russian doll is 3 ([2,3] => [5,4] => [6,7]).
```

Solution:
```cpp
class Solution {
public:
    int maxEnvelopes(vector<vector<int>>& envelopes) {
        
    }
};
```

## 1074. Number of Submatrices That Sum to Target

Given a matrix, and a target, return the number of non-empty submatrices that sum to target.

A submatrix x1, y1, x2, y2 is the set of all cells matrix[x][y] with x1 <= x <= x2 and y1 <= y <= y2.

Two submatrices (x1, y1, x2, y2) and (x1', y1', x2', y2') are different if they have some coordinate that is different: for example, if x1 != x1'.

 

Example 1:
```
Input: matrix = [[0,1,0],[1,1,1],[0,1,0]], target = 0
Output: 4
Explanation: The four 1x1 submatrices that only contain 0.
```
Example 2:
```
Input: matrix = [[1,-1],[-1,1]], target = 0
Output: 5
Explanation: The two 1x2 submatrices, plus the two 2x1 submatrices, 
plus the 2x2 submatrix.
``` 

Note:

- 1 <= matrix.length <= 300
- 1 <= matrix[0].length <= 300
- -1000 <= matrix[i] <= 1000
- -10^8 <= target <= 10^8

Solution:
```cpp
class Solution {
public:
    int numSubmatrixSumTarget(vector<vector<int>>& matrix, int target) {
        
    }
};
```

## 44. Wildcard Matching

Given an input string (s) and a pattern (p), implement wildcard pattern matching with support for '?' and '*'.

```
'?' Matches any single character.
'*' Matches any sequence of characters (including the empty sequence).
```

The matching should cover the entire input string (not partial).

Note:

- s could be empty and contains only lowercase letters a-z.
- p could be empty and contains only lowercase letters a-z, and characters like ? or *.

Example 1:
```
Input:
s = "aa"
p = "a"
Output: false
Explanation: "a" does not match the entire string "aa".
```
Example 2:
```
Input:
s = "aa"
p = "*"
Output: true
Explanation: '*' matches any sequence.
```
Example 3:
```
Input:
s = "cb"
p = "?a"
Output: false
Explanation: '?' matches 'c', but the second letter is 'a', 
which does not match 'b'.
```
Example 4:
```
Input:
s = "adceb"
p = "*a*b"
Output: true
Explanation: The first '*' matches the empty sequence, while the second '*' 
matches the substring "dce".
```

Example 5:
```
Input:
s = "acdcb"
p = "a*c?b"
Output: false
```

Solution:

```cpp

class Solution {
public:
    bool isMatch(string s, string p) {
        
    }
};
```

## 1049. Last Stone Weight II

We have a collection of rocks, each rock has a positive integer weight.

Each turn, we choose any two rocks and smash them together.  Suppose the stones have weights x and y with x <= y.  The result of this smash is:

- If x == y, both stones are totally destroyed;
- If x != y, the stone of weight x is totally destroyed, and the stone of weight y has new weight y-x.

At the end, there is at most 1 stone left.  Return the smallest possible weight of this stone (the weight is 0 if there are no stones left.)

 

Example 1:
```
Input: [2,7,4,1,8,1]
Output: 1
Explanation: 
We can combine 2 and 4 to get 2 so the array converts to [2,7,1,8,1] then,
we can combine 7 and 8 to get 1 so the array converts to [2,1,1,1] then,
we can combine 2 and 1 to get 1 so the array converts to [1,1,1] then,
we can combine 1 and 1 to get 0 so the array converts to [1] then that's the optimal value.
```

Note:

- 1 <= stones.length <= 30
- 1 <= stones[i] <= 100

Solution:
```cpp
class Solution {
public:
    int lastStoneWeightII(vector<int>& stones) {
        
    }
};
```

## 321. Create Maximum Number

Given two arrays of length m and n with digits 0-9 representing two numbers. Create the maximum number of length k <= m + n from digits of the two. The relative order of the digits from the same array must be preserved. Return an array of the k digits.

Note: You should try to optimize your time and space complexity.

Example 1:
```
Input:
nums1 = [3, 4, 6, 5]
nums2 = [9, 1, 2, 5, 8, 3]
k = 5
Output:
[9, 8, 6, 5, 3]
```
Example 2:
```
Input:
nums1 = [6, 7]
nums2 = [6, 0, 4]
k = 5
Output:
[6, 7, 6, 0, 4]
```
Example 3:
```
Input:
nums1 = [3, 9]
nums2 = [8, 9]
k = 3
Output:
[9, 8, 9]
```
Solution:
```cpp
class Solution {
public:
    vector<int> maxNumber(vector<int>& nums1, vector<int>& nums2, int k) {
        
    }
};
```

## 920. Number of Music Playlists

Your music player contains N different songs and she wants to listen to L (not necessarily different) songs during your trip.  You create a playlist so that:

Every song is played at least once
A song can only be played again only if K other songs have been played
Return the number of possible playlists.  As the answer can be very large, return it modulo 10^9 + 7.

Example 1:
```
Input: N = 3, L = 3, K = 1
Output: 6
Explanation: There are 6 possible playlists. 
[1, 2, 3], [1, 3, 2], [2, 1, 3], [2, 3, 1], [3, 1, 2], [3, 2, 1].
```
Example 2:
```
Input: N = 2, L = 3, K = 0
Output: 6
Explanation: There are 6 possible playlists. [1, 1, 2], [1, 2, 1], 
[2, 1, 1], [2, 2, 1], [2, 1, 2], [1, 2, 2]
```
Example 3:
```
Input: N = 2, L = 3, K = 1
Output: 2
Explanation: There are 2 possible playlists. [1, 2, 1], [2, 1, 2]
```

Note:

- 0 <= K < N <= L <= 100

Solution:
```cpp
class Solution {
public:
    int numMusicPlaylists(int N, int L, int K) {
        
    }
};
```

## 718. Maximum Length of Repeated Subarray

Given two integer arrays A and B, return the maximum length of an subarray that appears in both arrays.

Example 1:
```
Input:
A: [1,2,3,2,1]
B: [3,2,1,4,7]
Output: 3
Explanation: 
The repeated subarray with maximum length is [3, 2, 1].
```
 

Note:

- 1 <= len(A), len(B) <= 1000
- 0 <= A[i], B[i] < 100

Solution:
```cpp
class Solution {
public:
    int findLength(vector<int>& A, vector<int>& B) {
        
    }
};
```

## 847. Shortest Path Visiting All Nodes

An undirected, connected graph of N nodes (labeled 0, 1, 2, ..., N-1) is given as graph.

graph.length = N, and j != i is in the list graph[i] exactly once, if and only if nodes i and j are connected.

Return the length of the shortest path that visits every node. You may start and stop at any node, you may revisit nodes multiple times, and you may reuse edges.

 

Example 1:
```
Input: [[1,2,3],[0],[0],[0]]
Output: 4
Explanation: One possible path is [1,0,2,0,3]
```
Example 2:
```
Input: [[1],[0,2,4],[1,3,4],[2],[1,2]]
Output: 4
Explanation: One possible path is [0,1,4,2,3]
```

Note:

- 1<= graph.length <= 12
- 0 <= graph[i].length < graph.length

Solution:
```cpp
class Solution {
public:
    int shortestPathLength(vector<vector<int>>& graph) {
        
    }
};
```

## 1227. Airplane Seat Assignment Probability

n passengers board an airplane with exactly n seats. The first passenger has lost the ticket and picks a seat randomly. But after that, the rest of passengers will:

- Take their own seat if it is still available, 
- Pick other seats randomly when they find their seat occupied 

What is the probability that the n-th person can get his own seat?


Example 1:
```
Input: n = 1
Output: 1.00000
Explanation: The first person can only get the first seat.
```
Example 2:
```
Input: n = 2
Output: 0.50000
Explanation: The second person has a probability of 0.5 to get the second
seat (when first person gets the first seat).
```
 

Constraints:

- 1 <= n <= 10^5

Solution:
```cpp
class Solution {
public:
    double nthPersonGetsNthSeat(int n) {
        
    }
};
```

## 466. Count The Repetitions

Define S = [s,n] as the string S which consists of n connected strings s. For example, ["abc", 3] ="abcabcabc".

On the other hand, we define that string s1 can be obtained from string s2 if we can remove some characters from s2 such that it becomes s1. For example, “abc” can be obtained from “abdbec” based on our definition, but it can not be obtained from “acbbe”.

You are given two non-empty strings s1 and s2 (each at most 100 characters long) and two integers 0 ≤ n1 ≤ 106 and 1 ≤ n2 ≤ 106. Now consider the strings S1 and S2, where S1=[s1,n1] and S2=[s2,n2]. Find the maximum integer M such that [S2,M] can be obtained from S1.

Example:
```
Input:
s1="acb", n1=4
s2="ab", n2=2

Return:
2
```

Solution:
```cpp
class Solution {
public:
    int getMaxRepetitions(string s1, int n1, string s2, int n2) {
        
    }
};
```

## 983. Minimum Cost For Tickets

In a country popular for train travel, you have planned some train travelling one year in advance.  The days of the year that you will travel is given as an array days.  Each day is an integer from 1 to 365.

Train tickets are sold in 3 different ways:

- a 1-day pass is sold for costs[0] dollars;
- a 7-day pass is sold for costs[1] dollars;
- a 30-day pass is sold for costs[2] dollars.

The passes allow that many days of consecutive travel.  For example, if we get a 7-day pass on day 2, then we can travel for 7 days: day 2, 3, 4, 5, 6, 7, and 8.

Return the minimum number of dollars you need to travel every day in the given list of days.

 

Example 1:
```
Input: days = [1,4,6,7,8,20], costs = [2,7,15]
Output: 11
Explanation: 
For example, here is one way to buy passes that lets you travel your travel plan:
On day 1, you bought a 1-day pass for costs[0] = $2, which covered day 1.
On day 3, you bought a 7-day pass for costs[1] = $7, which covered days 3, 4, ..., 9.
On day 20, you bought a 1-day pass for costs[0] = $2, which covered day 20.
In total you spent $11 and covered all the days of your travel.
```
Example 2:
```
Input: days = [1,2,3,4,5,6,7,8,9,10,30,31], costs = [2,7,15]
Output: 17
Explanation: 
For example, here is one way to buy passes that lets you travel your travel plan:
On day 1, you bought a 30-day pass for costs[2] = $15 which covered days 1, 2, ..., 30.
On day 31, you bought a 1-day pass for costs[0] = $2 which covered day 31.
In total you spent $17 and covered all the days of your travel.
```



Note:

- 1 <= days.length <= 365
- 1 <= days[i] <= 365
- days is in strictly increasing order.
- costs.length == 3
- 1 <= costs[i] <= 1000

Solution:
```cpp
class Solution {
public:
    int mincostTickets(vector<int>& days, vector<int>& costs) {
        
    }
};
```

## 174. Dungeon Game

The demons had captured the princess (P) and imprisoned her in the bottom-right corner of a dungeon. The dungeon consists of M x N rooms laid out in a 2D grid. Our valiant knight (K) was initially positioned in the top-left room and must fight his way through the dungeon to rescue the princess.

The knight has an initial health point represented by a positive integer. If at any point his health point drops to 0 or below, he dies immediately.

Some of the rooms are guarded by demons, so the knight loses health (negative integers) upon entering these rooms; other rooms are either empty (0's) or contain magic orbs that increase the knight's health (positive integers).

In order to reach the princess as quickly as possible, the knight decides to move only rightward or downward in each step.

 

Write a function to determine the knight's minimum initial health so that he is able to rescue the princess.

For example, given the dungeon below, the initial health of the knight must be at least 7 if he follows the optimal path RIGHT-> RIGHT -> DOWN -> DOWN.

```
-2 (K)	-3	3
-5	-10	1
10	30	-5 (P)
 ```

Note:

- The knight's health has no upper bound.
- Any room can contain threats or power-ups, even the first room the knight enters and the bottom-right room where the princess is imprisoned.

Solution:
```cpp
class Solution {
public:
    int calculateMinimumHP(vector<vector<int>>& dungeon) {
        
    }
};
```

## 714. Best Time to Buy and Sell Stock with Transaction Fee

Your are given an array of integers prices, for which the i-th element is the price of a given stock on day i; and a non-negative integer fee representing a transaction fee.

You may complete as many transactions as you like, but you need to pay the transaction fee for each transaction. You may not buy more than 1 share of a stock at a time (ie. you must sell the stock share before you buy again.)

Return the maximum profit you can make.

Example 1:
```
Input: prices = [1, 3, 2, 8, 4, 9], fee = 2
Output: 8
Explanation: The maximum profit can be achieved by:
Buying at prices[0] = 1
Selling at prices[3] = 8
Buying at prices[4] = 4
Selling at prices[5] = 9
The total profit is ((8 - 1) - 2) + ((9 - 4) - 2) = 8.
```
Note:

- 0 < prices.length <= 50000.
- 0 < prices[i] < 50000.
- 0 <= fee < 50000.

Solution:
```cpp
class Solution {
public:
    int maxProfit(vector<int>& prices, int fee) {
        
    }
};
```

## 132. Palindrome Partitioning II

Given a string s, partition s such that every substring of the partition is a palindrome.

Return the minimum cuts needed for a palindrome partitioning of s.

Example:
```
Input: "aab"
Output: 1
Explanation: The palindrome partitioning ["aa","b"] could be produced using 1 cut.
```

Solution:
```cpp
class Solution {
public:
    int minCut(string s) {
        
    }
};
```

## 403. Frog Jump

A frog is crossing a river. The river is divided into x units and at each unit there may or may not exist a stone. The frog can jump on a stone, but it must not jump into the water.

Given a list of stones' positions (in units) in sorted ascending order, determine if the frog is able to cross the river by landing on the last stone. Initially, the frog is on the first stone and assume the first jump must be 1 unit.

If the frog's last jump was k units, then its next jump must be either k - 1, k, or k + 1 units. Note that the frog can only jump in the forward direction.

Note:

- The number of stones is ≥ 2 and is < 1,100.
- Each stone's position will be a non-negative integer < 231.
- The first stone's position is always 0.

Example 1:
```
[0,1,3,5,6,8,12,17]

There are a total of 8 stones.
The first stone at the 0th unit, second stone at the 1st unit,
third stone at the 3rd unit, and so on...
The last stone at the 17th unit.

Return true. The frog can jump to the last stone by jumping 
1 unit to the 2nd stone, then 2 units to the 3rd stone, then 
2 units to the 4th stone, then 3 units to the 6th stone, 
4 units to the 7th stone, and 5 units to the 8th stone.
```
Example 2:
```
[0,1,2,3,4,8,9,11]

Return false. There is no way to jump to the last stone as 
the gap between the 5th and 6th stone is too large.
```

Solution:
```cpp
class Solution {
public:
    bool canCross(vector<int>& stones) {
        
    }
};
```

## 304. Range Sum Query 2D - Immutable

Given a 2D matrix matrix, find the sum of the elements inside the rectangle defined by its upper left corner (row1, col1) and lower right corner (row2, col2).

![](https://leetcode.com/static/images/courses/range_sum_query_2d.png)

The above rectangle (with the red border) is defined by (row1, col1) = (2, 1) and (row2, col2) = (4, 3), which contains sum = 8.

Example:
```
Given matrix = [
  [3, 0, 1, 4, 2],
  [5, 6, 3, 2, 1],
  [1, 2, 0, 1, 5],
  [4, 1, 0, 1, 7],
  [1, 0, 3, 0, 5]
]

sumRegion(2, 1, 4, 3) -> 8
sumRegion(1, 1, 2, 2) -> 11
sumRegion(1, 2, 2, 4) -> 12
```
Note:
- You may assume that the matrix does not change.
- There are many calls to sumRegion function.
- You may assume that row1 ≤ row2 and col1 ≤ col2.

Solution:
```cpp
class NumMatrix {
public:
    NumMatrix(vector<vector<int>>& matrix) {
        
    }
    
    int sumRegion(int row1, int col1, int row2, int col2) {
        
    }
};

/**
 * Your NumMatrix object will be instantiated and called as such:
 * NumMatrix* obj = new NumMatrix(matrix);
 * int param_1 = obj->sumRegion(row1,col1,row2,col2);
 */
```

## 943. Find the Shortest Superstring

Given an array A of strings, find any smallest string that contains each string in A as a substring.

We may assume that no string in A is substring of another string in A.

 
Example 1:
```
Input: ["alex","loves","leetcode"]
Output: "alexlovesleetcode"
Explanation: All permutations of "alex","loves","leetcode" would also be accepted.
```
Example 2:
```
Input: ["catg","ctaagt","gcta","ttca","atgcatc"]
Output: "gctaagttcatgcatc"
```

Note:

- 1 <= A.length <= 12
- 1 <= A[i].length <= 20

Solution:
```cpp
class Solution {
public:
    string shortestSuperstring(vector<string>& A) {
        
    }
};
```

## 1314. Matrix Block Sum

Given a m * n matrix mat and an integer K, return a matrix answer where each answer[i][j] is the sum of all elements mat[r][c] for i - K <= r <= i + K, j - K <= c <= j + K, and (r, c) is a valid position in the matrix.

Example 1:
```
Input: mat = [[1,2,3],[4,5,6],[7,8,9]], K = 1
Output: [[12,21,16],[27,45,33],[24,39,28]]
```
Example 2:
```
Input: mat = [[1,2,3],[4,5,6],[7,8,9]], K = 2
Output: [[45,45,45],[45,45,45],[45,45,45]]
```

Constraints:

- m == mat.length
- n == mat[i].length
- 1 <= m, n, K <= 100
- 1 <= mat[i][j] <= 100

Solution:
```cpp
class Solution {
public:
    vector<vector<int>> matrixBlockSum(vector<vector<int>>& mat, int K) {
        
    }
};
```

## 740. Delete and Earn

Given an array nums of integers, you can perform operations on the array.

In each operation, you pick any nums[i] and delete it to earn nums[i] points. After, you must delete every element equal to nums[i] - 1 or nums[i] + 1.

You start with 0 points. Return the maximum number of points you can earn by applying such operations.

Example 1:
```
Input: nums = [3, 4, 2]
Output: 6
Explanation: 
Delete 4 to earn 4 points, consequently 3 is also deleted.
Then, delete 2 to earn 2 points. 6 total points are earned.
```

Example 2:
```
Input: nums = [2, 2, 3, 3, 3, 4]
Output: 9
Explanation: 
Delete 3 to earn 3 points, deleting both 2's and the 4.
Then, delete 3 again to earn 3 points, and 3 again to earn 3 points.
9 total points are earned.
``` 

Note:

- The length of nums is at most 20000.
- Each element nums[i] is an integer in the range [1, 10000].

Solution:
```cpp
class Solution {
public:
    int deleteAndEarn(vector<int>& nums) {
        
    }
};
```

## 638. Shopping Offers

In LeetCode Store, there are some kinds of items to sell. Each item has a price.

However, there are some special offers, and a special offer consists of one or more different kinds of items with a sale price.

You are given the each item's price, a set of special offers, and the number we need to buy for each item. The job is to output the lowest price you have to pay for exactly certain items as given, where you could make optimal use of the special offers.

Each special offer is represented in the form of an array, the last number represents the price you need to pay for this special offer, other numbers represents how many specific items you could get if you buy this offer.

You could use any of special offers as many times as you want.

Example 1:
```
Input: [2,5], [[3,0,5],[1,2,10]], [3,2]
Output: 14
Explanation: 
There are two kinds of items, A and B. Their prices are $2 and $5 respectively. 
In special offer 1, you can pay $5 for 3A and 0B
In special offer 2, you can pay $10 for 1A and 2B. 
You need to buy 3A and 2B, so you may pay $10 for 1A and 2B (special offer #2), 
and $4 for 2A.
```
Example 2:
```
Input: [2,3,4], [[1,1,0,4],[2,2,1,9]], [1,2,1]
Output: 11
Explanation: 
The price of A is $2, and $3 for B, $4 for C. 
You may pay $4 for 1A and 1B, and $9 for 2A ,2B and 1C. 
You need to buy 1A ,2B and 1C, so you may pay $4 for 1A and 1B 
(special offer #1), and $3 for 1B, $4 for 1C. 
You cannot add more items, though only $9 for 2A ,2B and 1C.
```

Note:
- There are at most 6 kinds of items, 100 special offers.
- For each item, you need to buy at most 6 of them.
- You are not allowed to buy more items than you want, even if that would lower the overall price.

Solution:
```cpp
class Solution {
public:
    int shoppingOffers(vector<int>& price, vector<vector<int>>& special, vector<int>& needs) {
        
    }
};
```

## 956. Tallest Billboard

You are installing a billboard and want it to have the largest height.  The billboard will have two steel supports, one on each side.  Each steel support must be an equal height.

You have a collection of rods which can be welded together.  For example, if you have rods of lengths 1, 2, and 3, you can weld them together to make a support of length 6.

Return the largest possible height of your billboard installation.  If you cannot support the billboard, return 0.

 

Example 1:
```
Input: [1,2,3,6]
Output: 6
Explanation: We have two disjoint subsets {1,2,3} and {6}, 
which have the same sum = 6.
```
Example 2:
```
Input: [1,2,3,4,5,6]
Output: 10
Explanation: We have two disjoint subsets {2,3,5} and {4,6}, 
which have the same sum = 10.
```

Example 3:
```
Input: [1,2]
Output: 0
Explanation: The billboard cannot be supported, so we return 0.
``` 

Note:

- 0 <= rods.length <= 20
- 1 <= rods[i] <= 1000
- The sum of rods is at most 5000.

Solution:
```cpp
class Solution {
public:
    int tallestBillboard(vector<int>& rods) {
        
    }
};
```

## 887. Super Egg Drop

You are given K eggs, and you have access to a building with N floors from 1 to N. 

Each egg is identical in function, and if an egg breaks, you cannot drop it again.

You know that there exists a floor F with 0 <= F <= N such that any egg dropped at a floor higher than F will break, and any egg dropped at or below floor F will not break.

Each move, you may take an egg (if you have an unbroken one) and drop it from any floor X (with 1 <= X <= N). 

Your goal is to know with certainty what the value of F is.

What is the minimum number of moves that you need to know with certainty what F is, regardless of the initial value of F?
 

Example 1:
```
Input: K = 1, N = 2
Output: 2
Explanation: 
Drop the egg from floor 1.  If it breaks, we know with certainty that F = 0.
Otherwise, drop the egg from floor 2.  If it breaks, we know with certainty that F = 1.
If it didn't break, then we know with certainty F = 2.
Hence, we needed 2 moves in the worst case to know what F is with certainty.
```
Example 2:
```
Input: K = 2, N = 6
Output: 3
```
Example 3:
```
Input: K = 3, N = 14
Output: 4
```

Note:

- 1 <= K <= 100
- 1 <= N <= 10000

Solution:
```cpp
class Solution {
public:
    int superEggDrop(int K, int N) {
        
    }
};
```

## 1048. Longest String Chain

Given a list of words, each word consists of English lowercase letters.

Let's say word1 is a predecessor of word2 if and only if we can add exactly one letter anywhere in word1 to make it equal to word2.  For example, "abc" is a predecessor of "abac".

A word chain is a sequence of words [word_1, word_2, ..., word_k] with k >= 1, where word_1 is a predecessor of word_2, word_2 is a predecessor of word_3, and so on.

Return the longest possible length of a word chain with words chosen from the given list of words.

Example 1:
```
Input: ["a","b","ba","bca","bda","bdca"]
Output: 4
Explanation: one of the longest word chain is "a","ba","bda","bdca".
```

Note:

- 1 <= words.length <= 1000
- 1 <= words[i].length <= 16
- words[i] only consists of English lowercase letters.

Solution:
```cpp
class Solution {
public:
    int longestStrChain(vector<string>& words) {
        
    }
};
```

## 256. Paint House

There are a row of n houses, each house can be painted with one of the three colors: red, blue or green. The cost of painting each house with a certain color is different. You have to paint all the houses such that no two adjacent houses have the same color.

The cost of painting each house with a certain color is represented by a n x 3 cost matrix. For example, costs[0][0] is the cost of painting house 0 with color red; costs[1][2] is the cost of painting house 1 with color green, and so on... Find the minimum cost to paint all houses.

Note:
All costs are positive integers.

Example:
```
Input: [[17,2,17],[16,16,5],[14,3,19]]
Output: 10
Explanation: Paint house 0 into blue, paint house 1 into green, paint house 2 into blue. 
             Minimum cost: 2 + 5 + 3 = 10.
```

Solution:
```cpp
class Solution {
public:
    int minCost(vector<vector<int>>& costs) {
        
    }
};
```

## 712. Minimum ASCII Delete Sum for Two Strings

Given two strings s1, s2, find the lowest ASCII sum of deleted characters to make two strings equal.

Example 1:
```
Input: s1 = "sea", s2 = "eat"
Output: 231
Explanation: Deleting "s" from "sea" adds the ASCII value of "s" (115) to the sum.
Deleting "t" from "eat" adds 116 to the sum.
At the end, both strings are equal, and 115 + 116 = 231 is the minimum sum possible
to achieve this.
```
Example 2:
```
Input: s1 = "delete", s2 = "leet"
Output: 403
Explanation: Deleting "dee" from "delete" to turn the string into "let",
adds 100[d]+101[e]+101[e] to the sum.  Deleting "e" from "leet" adds 101[e] to the sum.
At the end, both strings are equal to "let", and the answer is 100+101+101+101 = 403.
If instead we turned both strings into "lee" or "eet", we would get 
answers of 433 or 417, which are higher.
```
Note:

- 0 < s1.length, s2.length <= 1000.
- All elements of each string will have an ASCII value in [97, 122].

Solution:
```cpp
class Solution {
public:
    int minimumDeleteSum(string s1, string s2) {
        
    }
};
```

## 646. Maximum Length of Pair Chain

You are given n pairs of numbers. In every pair, the first number is always smaller than the second number.

Now, we define a pair (c, d) can follow another pair (a, b) if and only if b < c. Chain of pairs can be formed in this fashion.

Given a set of pairs, find the length longest chain which can be formed. You needn't use up all the given pairs. You can select pairs in any order.

Example 1:
```
Input: [[1,2], [2,3], [3,4]]
Output: 2
Explanation: The longest chain is [1,2] -> [3,4]
```
Note:
- The number of given pairs will be in the range [1, 1000].

Solution:
```cpp
class Solution {
public:
    int findLongestChain(vector<vector<int>>& pairs) {
        
    }
};
```

## 1000. Minimum Cost to Merge Stones

There are N piles of stones arranged in a row.  The i-th pile has stones[i] stones.

A move consists of merging exactly K consecutive piles into one pile, and the cost of this move is equal to the total number of stones in these K piles.

Find the minimum cost to merge all piles of stones into one pile.  If it is impossible, return -1.

 

Example 1:
```
Input: stones = [3,2,4,1], K = 2
Output: 20
Explanation: 
We start with [3, 2, 4, 1].
We merge [3, 2] for a cost of 5, and we are left with [5, 4, 1].
We merge [4, 1] for a cost of 5, and we are left with [5, 5].
We merge [5, 5] for a cost of 10, and we are left with [10].
The total cost was 20, and this is the minimum possible.
```
Example 2:
```
Input: stones = [3,2,4,1], K = 3
Output: -1
Explanation: After any merge operation, there are 2 piles left, 
and we can't merge anymore.  So the task is impossible.
```
Example 3:
```
Input: stones = [3,5,1,2,6], K = 3
Output: 25
Explanation: 
We start with [3, 5, 1, 2, 6].
We merge [5, 1, 2] for a cost of 8, and we are left with [3, 8, 6].
We merge [3, 8, 6] for a cost of 17, and we are left with [17].
The total cost was 25, and this is the minimum possible.
 ```

Note:

- 1 <= stones.length <= 30
- 2 <= K <= 30
- 1 <= stones[i] <= 100

Solution:
```cpp
class Solution {
public:
    int mergeStones(vector<int>& stones, int K) {
        
    }
};
```

## 975. Odd Even Jump

You are given an integer array A.  From some starting index, you can make a series of jumps.  The (1st, 3rd, 5th, ...) jumps in the series are called odd numbered jumps, and the (2nd, 4th, 6th, ...) jumps in the series are called even numbered jumps.

You may from index i jump forward to index j (with i < j) in the following way:

- During odd numbered jumps (ie. jumps 1, 3, 5, ...), you jump to the index j such that A[i] <= A[j] and A[j] is the smallest possible value.  If there are multiple such indexes j, you can only jump to the smallest such index j.
- During even numbered jumps (ie. jumps 2, 4, 6, ...), you jump to the index j such that A[i] >= A[j] and A[j] is the largest possible value.  If there are multiple such indexes j, you can only jump to the smallest such index j.
- (It may be the case that for some index i, there are no legal jumps.)
A starting index is good if, starting from that index, you can reach the end of the array (index A.length - 1) by jumping some number of times (possibly 0 or more than once.)

Return the number of good starting indexes.

 

Example 1:
```
Input: [10,13,12,14,15]
Output: 2
Explanation: 
From starting index i = 0, we can jump to i = 2 (since A[2] is the smallest among A[1], A[2], A[3], A[4] that is greater or equal to A[0]), then we can't jump any more.
From starting index i = 1 and i = 2, we can jump to i = 3, then we can't jump any more.
From starting index i = 3, we can jump to i = 4, so we've reached the end.
From starting index i = 4, we've reached the end already.
In total, there are 2 different starting indexes (i = 3, i = 4) where we can reach the end with some number of jumps.
```

Example 2:
```
Input: [2,3,1,1,4]
Output: 3
Explanation: 
From starting index i = 0, we make jumps to i = 1, i = 2, i = 3:

During our 1st jump (odd numbered), we first jump to i = 1 because A[1] 
is the smallest value in (A[1], A[2], A[3], A[4]) that is greater than 
or equal to A[0].

During our 2nd jump (even numbered), we jump from i = 1 to i = 2 because 
A[2] is the largest value in (A[2], A[3], A[4]) that is less than or equal 
to A[1].  A[3] is also the largest value, but 2 is a smaller index, so we 
can only jump to i = 2 and not i = 3.

During our 3rd jump (odd numbered), we jump from i = 2 to i = 3 because 
A[3] is the smallest value in (A[3], A[4]) that is greater than or equal 
to A[2].

We can't jump from i = 3 to i = 4, so the starting index i = 0 is not good.

In a similar manner, we can deduce that:
From starting index i = 1, we jump to i = 4, so we reach the end.
From starting index i = 2, we jump to i = 3, and then we can't jump anymore.
From starting index i = 3, we jump to i = 4, so we reach the end.
From starting index i = 4, we are already at the end.

In total, there are 3 different starting indexes (i = 1, i = 3, i = 4) 
where we can reach the end with some number of jumps.
```
Example 3:

Input: [5,1,3,4,2]
Output: 3
Explanation: 
We can reach the end from starting indexes 1, 2, and 4.
 

Note:

- 1 <= A.length <= 20000
- 0 <= A[i] < 100000

Solution:
```cpp
class Solution {
public:
    int oddEvenJumps(vector<int>& A) {
        
    }
};
```

## 903. Valid Permutations for DI Sequence

We are given S, a length n string of characters from the set {'D', 'I'}. (These letters stand for "decreasing" and "increasing".)

A valid permutation is a permutation P[0], P[1], ..., P[n] of integers {0, 1, ..., n}, such that for all i:

- If S[i] == 'D', then P[i] > P[i+1], and;
- If S[i] == 'I', then P[i] < P[i+1].

How many valid permutations are there?  Since the answer may be large, return your answer modulo 10^9 + 7.

 

Example 1:
```
Input: "DID"
Output: 5
Explanation: 
The 5 valid permutations of (0, 1, 2, 3) are:
(1, 0, 3, 2)
(2, 0, 3, 1)
(2, 1, 3, 0)
(3, 0, 2, 1)
(3, 1, 2, 0)
```

Note:

- 1 <= S.length <= 200
- S consists only of characters from the set {'D', 'I'}.

Solution:
```cpp
class Solution {
public:
    int numPermsDISequence(string S) {
        
    }
};
```

## 813. Largest Sum of Averages

We partition a row of numbers A into at most K adjacent (non-empty) groups, then our score is the sum of the average of each group. What is the largest score we can achieve?

Note that our partition must use every number in A, and that scores are not necessarily integers.

Example:
```
Input: 
A = [9,1,2,3,9]
K = 3
Output: 20
Explanation: 
The best choice is to partition A into [9], [1, 2, 3], [9]. 
The answer is 9 + (1 + 2 + 3) / 3 + 9 = 20.
We could have also partitioned A into [9, 1], [2], [3, 9], 
for example.
That partition would lead to a score of 5 + 2 + 6 = 13, which is worse.
```

Note:

- 1 <= A.length <= 100.
- 1 <= A[i] <= 10000.
- 1 <= K <= A.length.
- Answers within 10^-6 of the correct answer will be accepted as correct.

Solution: 
```cpp
class Solution {
public:
    double largestSumOfAverages(vector<int>& A, int K) {
        
    }
};
```

## 368. Largest Divisible Subset

Given a set of distinct positive integers, find the largest subset such that every pair (Si, Sj) of elements in this subset satisfies:

Si % Sj = 0 or Sj % Si = 0.

If there are multiple solutions, return any subset is fine.

Example 1:
```
Input: [1,2,3]
Output: [1,2] (of course, [1,3] will also be ok)
```

Example 2:
```
Input: [1,2,4,8]
Output: [1,2,4,8]
```

Solution:
```cpp
class Solution {
public:
    vector<int> largestDivisibleSubset(vector<int>& nums) {
        
    }
};
```

## 213. House Robber II

You are a professional robber planning to rob houses along a street. Each house has a certain amount of money stashed. All houses at this place are arranged in a circle. That means the first house is the neighbor of the last one. Meanwhile, adjacent houses have security system connected and it will automatically contact the police if two adjacent houses were broken into on the same night.

Given a list of non-negative integers representing the amount of money of each house, determine the maximum amount of money you can rob tonight without alerting the police.

Example 1:
```
Input: [2,3,2]
Output: 3
Explanation: You cannot rob house 1 (money = 2) and then rob house 3 (money = 2),
             because they are adjacent houses.
```

Example 2:
```
Input: [1,2,3,1]
Output: 4
Explanation: Rob house 1 (money = 1) and then rob house 3 (money = 3).
             Total amount you can rob = 1 + 3 = 4.
```

Solution:
```cpp
class Solution {
public:
    int rob(vector<int>& nums) {
        
    }
};
```

## 494. Target Sum

You are given a list of non-negative integers, a1, a2, ..., an, and a target, S. Now you have 2 symbols + and -. For each integer, you should choose one from + and - as its new symbol.

Find out how many ways to assign symbols to make sum of integers equal to target S.

Example 1:
```
Input: nums is [1, 1, 1, 1, 1], S is 3. 
Output: 5
Explanation: 

-1+1+1+1+1 = 3
+1-1+1+1+1 = 3
+1+1-1+1+1 = 3
+1+1+1-1+1 = 3
+1+1+1+1-1 = 3

There are 5 ways to assign symbols to make the sum of nums be target 3.
```

Constraints:

- The length of the given array is positive and will not exceed 20.
- The sum of elements in the given array will not exceed 1000.
- Your output answer is guaranteed to be fitted in a 32-bit integer.

Solution:
```cpp
class Solution {
public:
    int findTargetSumWays(vector<int>& nums, int S) {
        
    }
};
```

## 377. Combination Sum IV

Given an integer array with all positive numbers and no duplicates, find the number of possible combinations that add up to a positive integer target.

Example:
```
nums = [1, 2, 3]
target = 4

The possible combination ways are:
(1, 1, 1, 1)
(1, 1, 2)
(1, 2, 1)
(1, 3)
(2, 1, 1)
(2, 2)
(3, 1)

Note that different sequences are counted as different combinations.

Therefore the output is 7.
 ```

Follow up:

What if negative numbers are allowed in the given array?

How does it change the problem?

What limitation we need to add to the question to allow negative numbers?

Credits:

Special thanks to @pbrother for adding this problem and creating all test cases.

Solution:
```cpp
class Solution {
public:
    int combinationSum4(vector<int>& nums, int target) {
        
    }
};
```

## 1027. Longest Arithmetic Sequence

Given an array A of integers, return the length of the longest arithmetic subsequence in A.

Recall that a subsequence of A is a list A[i_1], A[i_2], ..., A[i_k] with 0 <= i_1 < i_2 < ... < i_k <= A.length - 1, and that a sequence B is arithmetic if B[i+1] - B[i] are all the same value (for 0 <= i < B.length - 1).

 

Example 1:
```
Input: [3,6,9,12]
Output: 4
Explanation: 
The whole array is an arithmetic sequence with steps of length = 3.
```
Example 2:
```
Input: [9,4,7,2,10]
Output: 3
Explanation: 
The longest arithmetic subsequence is [4,7,10].
```
Example 3:
```
Input: [20,1,15,3,10,5,8]
Output: 4
Explanation: 
The longest arithmetic subsequence is [20,15,10,5].
``` 

Note:

- 2 <= A.length <= 2000
- 0 <= A[i] <= 10000

Solution:
```cpp
class Solution {
public:
    int longestArithSeqLength(vector<int>& A) {
        
    }
};
```

## 416. Partition Equal Subset Sum

Given a non-empty array containing only positive integers, find if the array can be partitioned into two subsets such that the sum of elements in both subsets is equal.

Note:

- Each of the array element will not exceed 100.
- The array size will not exceed 200.
 

Example 1:
```
Input: [1, 5, 11, 5]

Output: true

Explanation: The array can be partitioned as [1, 5, 5] and [11].
``` 

Example 2:
```
Input: [1, 2, 3, 5]

Output: false

Explanation: The array cannot be partitioned into equal sum subsets.
```

Soluton:
```cpp
class Solution {
public:
    bool canPartition(vector<int>& nums) {
        
    }
};
```

## 464. Can I Win

In the "100 game," two players take turns adding, to a running total, any integer from 1..10. The player who first causes the running total to reach or exceed 100 wins.

What if we change the game so that players cannot re-use integers?

For example, two players might take turns drawing from a common pool of numbers of 1..15 without replacement until they reach a total >= 100.

Given an integer maxChoosableInteger and another integer desiredTotal, determine if the first player to move can force a win, assuming both players play optimally.

You can always assume that maxChoosableInteger will not be larger than 20 and desiredTotal will not be larger than 300.

Example
```
Input:
maxChoosableInteger = 10
desiredTotal = 11

Output:
false

Explanation:
No matter which integer the first player choose, the first player will lose.
The first player can choose an integer from 1 up to 10.
If the first player choose 1, the second player can only choose integers from 2 up to 10.
The second player will win by choosing 10 and get a total = 11, which is >= desiredTotal.
Same with other integers chosen by the first player, the second player will always win.
```

Solution:
```cpp
class Solution {
public:
    bool canIWin(int maxChoosableInteger, int desiredTotal) {
        
    }
};
```

## 1105. Filling Bookcase Shelves

We have a sequence of books: the i-th book has thickness books[i][0] and height books[i][1].

We want to place these books in order onto bookcase shelves that have total width shelf_width.

We choose some of the books to place on this shelf (such that the sum of their thickness is <= shelf_width), then build another level of shelf of the bookcase so that the total height of the bookcase has increased by the maximum height of the books we just put down.  We repeat this process until there are no more books to place.

Note again that at each step of the above process, the order of the books we place is the same order as the given sequence of books.  For example, if we have an ordered list of 5 books, we might place the first and second book onto the first shelf, the third book on the second shelf, and the fourth and fifth book on the last shelf.

Return the minimum possible height that the total bookshelf can be after placing shelves in this manner.

Example 1:

![](https://assets.leetcode.com/uploads/2019/06/24/shelves.png)

```
Input: books = [[1,1],[2,3],[2,3],[1,1],[1,1],[1,1],[1,2]], shelf_width = 4
Output: 6
Explanation:
The sum of the heights of the 3 shelves are 1 + 3 + 2 = 6.
Notice that book number 2 does not have to be on the first shelf.
```

Constraints:

- 1 <= books.length <= 1000
- 1 <= books[i][0] <= shelf_width <= 1000
- 1 <= books[i][1] <= 1000

## 689. Maximum Sum of 3 Non-Overlapping Subarrays

In a given array nums of positive integers, find three non-overlapping subarrays with maximum sum.

Each subarray will be of size k, and we want to maximize the sum of all 3*k entries.

Return the result as a list of indices representing the starting position of each interval (0-indexed). If there are multiple answers, return the lexicographically smallest one.

Example:
```
Input: [1,2,1,2,6,7,5,1], 2
Output: [0, 3, 5]
Explanation: Subarrays [1, 2], [2, 6], [7, 5] correspond to 
the starting indices [0, 3, 5].
We could have also taken [2, 1], but an answer of [1, 3, 5] 
would be lexicographically larger.
```

Note:

- nums.length will be between 1 and 20000.
- nums[i] will be between 1 and 65535.
- k will be between 1 and floor(nums.length / 3).

Solution:
```cpp
class Solution {
public:
    vector<int> maxSumOfThreeSubarrays(vector<int>& nums, int k) {
        
    }
};
```

## 964. Least Operators to Express Number

Given a single positive integer x, we will write an expression of the form x (op1) x (op2) x (op3) x ... where each operator op1, op2, etc. is either addition, subtraction, multiplication, or division (+, -, *, or /).  For example, with x = 3, we might write 3 * 3 / 3 + 3 - 3 which is a value of 3.

When writing such an expression, we adhere to the following conventions:

- The division operator (/) returns rational numbers.
- There are no parentheses placed anywhere.
- We use the usual order of operations: multiplication and division happens before addition and subtraction.
- It's not allowed to use the unary negation operator (-).  For example, "x - x" is a valid expression as it only uses subtraction, but "-x + x" is not because it uses negation.

We would like to write an expression with the least number of operators such that the expression equals the given target.  Return the least number of operators used.

 

Example 1:
```
Input: x = 3, target = 19
Output: 5
Explanation: 3 * 3 + 3 * 3 + 3 / 3. 
The expression contains 5 operations.
```
Example 2:
```
Input: x = 5, target = 501
Output: 8
Explanation: 5 * 5 * 5 * 5 - 5 * 5 * 5 + 5 / 5.  
The expression contains 8 operations.
```
Example 3:
```
Input: x = 100, target = 100000000
Output: 3
Explanation: 100 * 100 * 100 * 100.  
The expression contains 3 operations.
``` 

Note:

- 2 <= x <= 100
- 1 <= target <= 2 * 10^8

Solution:
```cpp
class Solution {
public:
    int leastOpsExpressTarget(int x, int target) {
        
    }
};
```

## 474. Ones and Zeroes

Given an array, strs, with strings consisting of only 0s and 1s. Also two integers m and n.

Now your task is to find the maximum number of strings that you can form with given m 0s and n 1s. Each 0 and 1 can be used at most once.

 

Example 1:
```
Input: strs = ["10","0001","111001","1","0"], m = 5, n = 3
Output: 4
Explanation: This are totally 4 strings can be formed by 
the using of 5 0s and 3 1s, which are "10","0001","1","0".
```
Example 2:
```
Input: strs = ["10","0","1"], m = 1, n = 1
Output: 2
Explanation: You could form "10", but then you'd have
nothing left. Better form "0" and "1".
 ```

Constraints:

- 1 <= strs.length <= 600
- 1 <= strs[i].length <= 100
- strs[i] consists only of digits '0' and '1'.
- 1 <= m, n <= 100

Solution:
```cpp
class Solution {
public:
    int findMaxForm(vector<string>& strs, int m, int n) {
        
    }
};
```

## 935. Knight Dialer

A chess knight can move as indicated in the chess diagram below:

![](https://assets.leetcode.com/uploads/2018/10/30/keypad.png)

This time, we place our chess knight on any numbered key of a phone pad (indicated above), and the knight makes N-1 hops.  Each hop must be from one key to another numbered key.

Each time it lands on a key (including the initial placement of the knight), it presses the number of that key, pressing N digits total.

How many distinct numbers can you dial in this manner?

Since the answer may be large, output the answer modulo 10^9 + 7.

 

Example 1:
```
Input: 1
Output: 10
```
Example 2:
```
Input: 2
Output: 20
```
Example 3:
```
Input: 3
Output: 46
``` 

Note:

- 1 <= N <= 5000

Solution:
```cpp
class Solution {
public:
    int knightDialer(int N) {
        
    }
};
```

## 276. Paint Fence

There is a fence with n posts, each post can be painted with one of the k colors.

You have to paint all the posts such that no more than two adjacent fence posts have the same color.

Return the total number of ways you can paint the fence.

Note:
n and k are non-negative integers.

Example:
```
Input: n = 3, k = 2
Output: 6
Explanation: Take c1 as color 1, c2 as color 2. All possible ways are:

            post1  post2  post3      
 -----      -----  -----  -----       
   1         c1     c1     c2 
   2         c1     c2     c1 
   3         c1     c2     c2 
   4         c2     c1     c1  
   5         c2     c1     c2
   6         c2     c2     c1
```

Solution:
```cpp
class Solution {
public:
    int numWays(int n, int k) {
        
    }
};
```

## 688. Knight Probability in Chessboard

On an NxN chessboard, a knight starts at the r-th row and c-th column and attempts to make exactly K moves. The rows and columns are 0 indexed, so the top-left square is (0, 0), and the bottom-right square is (N-1, N-1).

A chess knight has 8 possible moves it can make, as illustrated below. Each move is two squares in a cardinal direction, then one square in an orthogonal direction.
 
![](https://assets.leetcode.com/uploads/2018/10/12/knight.png)

Each time the knight is to move, it chooses one of eight possible moves uniformly at random (even if the piece would go off the chessboard) and moves there.

The knight continues moving until it has made exactly K moves or has moved off the chessboard. Return the probability that the knight remains on the board after it has stopped moving.

 

Example:
```
Input: 3, 2, 0, 0
Output: 0.0625
Explanation: There are two moves (to (1,2), (2,1)) 
that will keep the knight on the board.
From each of those positions, there are also two moves 
that will keep the knight on the board.
The total probability the knight stays on the board 
is 0.0625.
 ```

Note:

- N will be between 1 and 25.
- K will be between 0 and 100.
- The knight always initially starts on the board.

Solution:
```cpp
class Solution {
public:
    double knightProbability(int N, int K, int r, int c) {
        
    }
};
```

## 650. 2 Keys Keyboard

Initially on a notepad only one character 'A' is present. You can perform two operations on this notepad for each step:

- Copy All: You can copy all the characters present on the notepad (partial copy is not allowed).
- Paste: You can paste the characters which are copied last time.
 

Given a number n. You have to get exactly n 'A' on the notepad by performing the minimum number of steps permitted. Output the minimum number of steps to get n 'A'.

Example 1:
```
Input: 3
Output: 3
Explanation:
Intitally, we have one character 'A'.
In step 1, we use Copy All operation.
In step 2, we use Paste operation to get 'AA'.
In step 3, we use Paste operation to get 'AAA'.
``` 

Note:

- The n will be in the range [1, 1000].

Solution:
```cpp
class Solution {
public:
    int minSteps(int n) {
        
    }
};
```

## 664. Strange Printer

There is a strange printer with the following two special requirements:

- The printer can only print a sequence of the same character each time.
- At each turn, the printer can print new characters starting from and ending at any places, and will cover the original existing characters.

Given a string consists of lower English letters only, your job is to count the minimum number of turns the printer needed in order to print it.

Example 1:
```
Input: "aaabbb"
Output: 2
Explanation: Print "aaa" first and then print "bbb".
```
Example 2:
```
Input: "aba"
Output: 2
Explanation: Print "aaa" first and then print "b" from 
the second place of the string, which will cover the 
existing character 'a'.
```
Hint: Length of the given string will not exceed 100.

Solution:
```cpp
class Solution {
public:
    int strangePrinter(string s) {
        
    }
};
```

## 673. Number of Longest Increasing Subsequence

Given an unsorted array of integers, find the number of longest increasing subsequence.

Example 1:
```
Input: [1,3,5,4,7]
Output: 2
Explanation: The two longest increasing subsequence are 
[1, 3, 4, 7] and [1, 3, 5, 7].
```
Example 2:
```
Input: [2,2,2,2,2]
Output: 5
Explanation: The length of longest continuous increasing
subsequence is 1, and there are 5 subsequences' length is 
1, so output 5.
```
Note: Length of the given array will be not exceed 2000 and the answer is guaranteed to be fit in 32-bit signed int.

Solution:
```cpp
class Solution {
public:
    int findNumberOfLIS(vector<int>& nums) {
        
    }
};
```

## 63. Unique Paths II

A robot is located at the top-left corner of a m x n grid (marked 'Start' in the diagram below).

The robot can only move either down or right at any point in time. The robot is trying to reach the bottom-right corner of the grid (marked 'Finish' in the diagram below).

Now consider if some obstacles are added to the grids. How many unique paths would there be?

![](https://assets.leetcode.com/uploads/2018/10/22/robot_maze.png)

An obstacle and empty space is marked as 1 and 0 respectively in the grid.

Note: m and n will be at most 100.

Example 1:
```
Input:
[
  [0,0,0],
  [0,1,0],
  [0,0,0]
]
Output: 2
Explanation:
There is one obstacle in the middle of the 3x3 grid above.
There are two ways to reach the bottom-right corner:
1. Right -> Right -> Down -> Down
2. Down -> Down -> Right -> Right
```

Solution:
```cpp
class Solution {
public:
    int uniquePathsWithObstacles(vector<vector<int>>& obstacleGrid) {
        
    }
};
```

## 486. Predict the Winner

Given an array of scores that are non-negative integers. Player 1 picks one of the numbers from either end of the array followed by the player 2 and then player 1 and so on. Each time a player picks a number, that number will not be available for the next player. This continues until all the scores have been chosen. The player with the maximum score wins.

Given an array of scores, predict whether player 1 is the winner. You can assume each player plays to maximize his score.

Example 1:
```
Input: [1, 5, 2]
Output: False
Explanation: Initially, player 1 can choose between 1 and 2. 

If he chooses 2 (or 1), then player 2 can choose from 1 (or 2) 
and 5. If player 2 chooses 5, then player 1 will be left with 1 (or 2). 

So, final score of player 1 is 1 + 2 = 3, and player 2 is 5. 
Hence, player 1 will never be the winner and you need to return False.
```

Example 2:
```
Input: [1, 5, 233, 7]
Output: True
Explanation: Player 1 first chooses 1. Then player 2 have to choose 
between 5 and 7. No matter which number player 2 choose, player 1 
can choose 233.
Finally, player 1 has more score (234) than player 2 (12), so you 
need to return True representing player1 can win.
```

Note:
- 1 <= length of the array <= 20.
- Any scores in the given array are non-negative integers and will not exceed 10,000,000.
- If the scores of both players are equal, then player 1 is still the winner.

Solution:
```cpp
class Solution {
public:
    bool PredictTheWinner(vector<int>& nums) {
        
    }
};
```

## 472. Concatenated Words

Given a list of words (without duplicates), please write a program that returns all concatenated words in the given list of words.
A concatenated word is defined as a string that is comprised entirely of at least two shorter words in the given array.

Example:
```
Input: [
    "cat","cats","catsdogcats","dog","dogcatsdog",
    "hippopotamuses","rat","ratcatdogcat"
]

Output: ["catsdogcats","dogcatsdog","ratcatdogcat"]

Explanation: "catsdogcats" can be concatenated by "cats", "dog" and "cats"; 
 "dogcatsdog" can be concatenated by "dog", "cats" and "dog"; 
"ratcatdogcat" can be concatenated by "rat", "cat", "dog" and "cat".
```
Note:
- The number of elements of the given array will not exceed 10,000
- The length sum of elements in the given array will not exceed 600,000.
- All the input string will only include lower case letters.
- The returned elements order does not matter.

Solution:
```cpp
class Solution {
public:
    vector<string> findAllConcatenatedWordsInADict(vector<string>& words) {
        
    }
};
```

## 376. Wiggle Subsequence

A sequence of numbers is called a wiggle sequence if the differences between successive numbers strictly alternate between positive and negative. The first difference (if one exists) may be either positive or negative. A sequence with fewer than two elements is trivially a wiggle sequence.

For example, [1,7,4,9,2,5] is a wiggle sequence because the differences (6,-3,5,-7,3) are alternately positive and negative. In contrast, [1,4,7,2,5] and [1,7,4,5,5] are not wiggle sequences, the first because its first two differences are positive and the second because its last difference is zero.

Given a sequence of integers, return the length of the longest subsequence that is a wiggle sequence. A subsequence is obtained by deleting some number of elements (eventually, also zero) from the original sequence, leaving the remaining elements in their original order.

Example 1:
```
Input: [1,7,4,9,2,5]
Output: 6
Explanation: The entire sequence is a wiggle sequence.
```

Example 2:
```
Input: [1,17,5,10,13,15,10,5,16,8]
Output: 7
Explanation: There are several subsequences that achieve 
this length. One is [1,17,10,13,10,16,8].
```
Example 3:
```
Input: [1,2,3,4,5,6,7,8,9]
Output: 2
```
Follow up:
Can you do it in O(n) time?

Solution:
```cpp

class Solution {
public:
    int wiggleMaxLength(vector<int>& nums) {
        
    }
};
```

## 931. Minimum Falling Path Sum

Given a square array of integers A, we want the minimum sum of a falling path through A.

A falling path starts at any element in the first row, and chooses one element from each row.  The next row's choice must be in a column that is different from the previous row's column by at most one.


Example 1:
```
Input: [[1,2,3],[4,5,6],[7,8,9]]
Output: 12
Explanation: 
The possible falling paths are:
```
- [1,4,7], [1,4,8], [1,5,7], [1,5,8], [1,5,9]
- [2,4,7], [2,4,8], [2,5,7], [2,5,8], [2,5,9], [2,6,8], [2,6,9]
- [3,5,7], [3,5,8], [3,5,9], [3,6,8], [3,6,9]

The falling path with the smallest sum is [1,4,7], so the answer is 12.

 

Constraints:

- 1 <= A.length == A[0].length <= 100
- -100 <= A[i][j] <= 100

Solution:
```cpp
class Solution {
public:
    int minFallingPathSum(vector<vector<int>>& A) {
        
    }
};
```

## 898. Bitwise ORs of Subarrays

We have an array A of non-negative integers.

For every (contiguous) subarray B = [A[i], A[i+1], ..., A[j]] (with i <= j), we take the bitwise OR of all the elements in B, obtaining a result A[i] | A[i+1] | ... | A[j].

Return the number of possible results.  (Results that occur more than once are only counted once in the final answer.)

 

Example 1:
```
Input: [0]
Output: 1
Explanation: 
There is only one possible result: 0.
```
Example 2:
```
Input: [1,1,2]
Output: 3
Explanation: 
The possible subarrays are [1], [1], [2], [1, 1],
[1, 2], [1, 1, 2].
These yield the results 1, 1, 2, 1, 3, 3.
There are 3 unique values, so the answer is 3.
```
Example 3:
```
Input: [1,2,4]
Output: 6
Explanation: 
The possible results are 1, 2, 3, 4, 6, and 7.
 ```

Note:

- 1 <= A.length <= 50000
- 0 <= A[i] <= 10^9

Solution:
```cpp
class Solution {
public:
    int subarrayBitwiseORs(vector<int>& A) {
        
    }
};
```

## 1039. Minimum Score Triangulation of Polygon

Given N, consider a convex N-sided polygon with vertices labelled A[0], A[i], ..., A[N-1] in clockwise order.

Suppose you triangulate the polygon into N-2 triangles.  For each triangle, the value of that triangle is the product of the labels of the vertices, and the total score of the triangulation is the sum of these values over all N-2 triangles in the triangulation.

Return the smallest possible total score that you can achieve with some triangulation of the polygon.

 

Example 1:
```
Input: [1,2,3]
Output: 6
Explanation: The polygon is already triangulated,
and the score of the only triangle is 6.
```
Example 2:

![](https://assets.leetcode.com/uploads/2019/05/01/minimum-score-triangulation-of-polygon-1.png)

```
Input: [3,7,4,5]
Output: 144
Explanation: There are two triangulations, with possible
scores: 3*7*5 + 4*5*7 = 245, or 3*4*5 + 3*4*7 = 144. 
The minimum score is 144.
```
Example 3:
```
Input: [1,3,1,4,1,5]
Output: 13
Explanation: The minimum score triangulation has 
score 1*1*3 + 1*1*4 + 1*1*5 + 1*1*1 = 13.
``` 

Note:

- 3 <= A.length <= 50
- 1 <= A[i] <= 100

Solution:
```cpp
class Solution {
public:
    int minScoreTriangulation(vector<int>& A) {
        
    }
};
```

## 801. Minimum Swaps To Make Sequences Increasing

We have two integer sequences A and B of the same non-zero length.

We are allowed to swap elements A[i] and B[i].  Note that both elements are in the same index position in their respective sequences.

At the end of some number of swaps, A and B are both strictly increasing.  (A sequence is strictly increasing if and only if A[0] < A[1] < A[2] < ... < A[A.length - 1].)

Given A and B, return the minimum number of swaps to make both sequences strictly increasing.  It is guaranteed that the given input always makes it possible.

Example:
```
Input: A = [1,3,5,4], B = [1,2,3,7]
Output: 1
Explanation: 
Swap A[3] and B[3].  Then the sequences are:
A = [1, 3, 5, 7] and B = [1, 2, 3, 4]
which are both strictly increasing.
```
Note:

- A, B are arrays with the same length, and that length will be in the range [1, 1000].
- A[i], B[i] are integer values in the range [0, 2000].

Solution:
```cpp
class Solution {
public:
    int minSwap(vector<int>& A, vector<int>& B) {
        
    }
};
```

## 361. Bomb Enemy

Given a 2D grid, each cell is either a wall 'W', an enemy 'E' or empty '0' (the number zero), return the maximum enemies you can kill using one bomb.
The bomb kills all the enemies in the same row and column from the planted point until it hits the wall since the wall is too strong to be destroyed.
Note: You can only put the bomb at an empty cell.

Example:
```
Input: [
   ["0","E","0","0"],["E","0","W","E"],["0","E","0","0"]]
Output: 3 
Explanation: For the given grid,

0 E 0 0 
E 0 W E 
0 E 0 0

Placing a bomb at (1,1) kills 3 enemies.
```

Solution:
```cpp
class Solution {
public:
    int maxKilledEnemies(vector<vector<char>>& grid) {
        
    }
};
```

## 968. Binary Tree Cameras

Given a binary tree, we install cameras on the nodes of the tree. 

Each camera at a node can monitor its parent, itself, and its immediate children.

Calculate the minimum number of cameras needed to monitor all nodes of the tree.

 

Example 1:

![](https://assets.leetcode.com/uploads/2018/12/29/bst_cameras_01.png)
```        
Input: [0,0,null,0,0]
Output: 1
Explanation: One camera is enough to monitor all nodes if placed as shown.
```
Example 2:

![](https://assets.leetcode.com/uploads/2018/12/29/bst_cameras_02.png)
 
```
Input: [0,0,null,0,null,0,null,null,0]
Output: 2
Explanation: At least two cameras are needed 
to monitor all nodes of the tree. The above 
image shows one of the valid configurations 
of camera placement.
```
Note:

- The number of nodes in the given tree will be in the range [1, 1000].
- Every node has value 0.

Solution:
```cpp
/**
 * Definition for a binary tree node.
 * struct TreeNode {
 *     int val;
 *     TreeNode *left;
 *     TreeNode *right;
 *     TreeNode() : val(0), left(nullptr), right(nullptr) {}
 *     TreeNode(int x) : val(x), left(nullptr), right(nullptr) {}
 *     TreeNode(int x, TreeNode *left, TreeNode *right) : val(x), left(left), right(right) {}
 * };
 */
class Solution {
public:
    int minCameraCover(TreeNode* root) {
        
    }
};
```

838. Push Dominoes
Medium

543

63

Add to List

Share
There are N dominoes in a line, and we place each domino vertically upright.

In the beginning, we simultaneously push some of the dominoes either to the left or to the right.

![](https://s3-lc-upload.s3.amazonaws.com/uploads/2018/05/18/domino.png)

After each second, each domino that is falling to the left pushes the adjacent domino on the left.

Similarly, the dominoes falling to the right push their adjacent dominoes standing on the right.

When a vertical domino has dominoes falling on it from both sides, it stays still due to the balance of the forces.

For the purposes of this question, we will consider that a falling domino expends no additional force to a falling or already fallen domino.

Given a string "S" representing the initial state. S[i] = 'L', if the i-th domino has been pushed to the left; S[i] = 'R', if the i-th domino has been pushed to the right; S[i] = '.', if the i-th domino has not been pushed.

Return a string representing the final state. 

Example 1:
```
Input: ".L.R...LR..L.."
Output: "LL.RR.LLRRLL.."
```
Example 2:
```
Input: "RR.L"
Output: "RR.L"
Explanation: The first domino expends no additional
force on the second domino.
```
Note:

- 0 <= N <= 10^5
- String dominoes contains only 'L', 'R' and '.'

Solution:
```cpp
class Solution {
public:
    string pushDominoes(string dominoes) {
        
    }
};
```
