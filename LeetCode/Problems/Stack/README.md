
# Stack

## 1021. Remove Outermost Parentheses

A valid parentheses string is either empty (""), "(" + A + ")", or A + B, where A and B are valid parentheses strings, and + represents string concatenation.  For example, "", "()", "(())()", and "(()(()))" are all valid parentheses strings.

A valid parentheses string S is primitive if it is nonempty, and there does not exist a way to split it into S = A+B, with A and B nonempty valid parentheses strings.

Given a valid parentheses string S, consider its primitive decomposition: S = P_1 + P_2 + ... + P_k, where P_i are primitive valid parentheses strings.

Return S after removing the outermost parentheses of every primitive string in the primitive decomposition of S.

Example 1:
```
Input: "(()())(())"
Output: "()()()"
Explanation: 
The input string is "(()())(())", 
with primitive decomposition "(()())" + "(())".
After removing outer parentheses of each part, 
this is "()()" + "()" = "()()()".
```

Example 2:
```
Input: "(()())(())(()(()))"
Output: "()()()()(())"
Explanation: 
The input string is "(()())(())(()(()))", 
with primitive decomposition "(()())" + "(())" + "(()(()))".
After removing outer parentheses of each part, 
this is "()()" + "()" + "()(())" = "()()()()(())".
```

Example 3:
```
Input: "()()"
Output: ""
Explanation: 
The input string is "()()", with primitive decomposition "()" + "()".
After removing outer parentheses of each part, this is "" + "" = "".
```

Note:

- S.length <= 10000
- S[i] is "(" or ")"
- S is a valid parentheses string

Solution:
```cpp
class Solution {
public:
    string removeOuterParentheses(string S) {
        
    }
};
```

## 1441. Build an Array With Stack Operations

Given an array target and an integer n. In each iteration, you will read a number from  list = {1,2,3..., n}.

Build the target array using the following operations:

- Push: Read a new element from the beginning list, and push it in the array.
- Pop: delete the last element of the array.
- If the target array is already built, stop reading more elements.

You are guaranteed that the target array is strictly increasing, only containing numbers between 1 to n inclusive.

Return the operations to build the target array.

You are guaranteed that the answer is unique.

Example 1:
```
Input: target = [1,3], n = 3
Output: ["Push","Push","Pop","Push"]
Explanation: 
Read number 1 and automatically push in the array -> [1]
Read number 2 and automatically push in the array then Pop it -> [1]
Read number 3 and automatically push in the array -> [1,3]
```

Example 2:
```
Input: target = [1,2,3], n = 3
Output: ["Push","Push","Push"]
```
Example 3:
```
Input: target = [1,2], n = 4
Output: ["Push","Push"]
Explanation: You only need to read the first 2 numbers and stop.
```
Example 4:
```
Input: target = [2,3,4], n = 4
Output: ["Push","Pop","Push","Push","Push"]
```

Constraints:

- 1 <= target.length <= 100
- 1 <= target[i] <= 100
- 1 <= n <= 100
- target is strictly increasing.

Solution:
```cpp
class Solution {
public:
    vector<string> buildArray(vector<int>& target, int n) {
        
    }
};
```


## 1047. Remove All Adjacent Duplicates In String

Given a string S of lowercase letters, a duplicate removal consists of choosing two adjacent and equal letters, and removing them.

We repeatedly make duplicate removals on S until we no longer can.

Return the final string after all such duplicate removals have been made.  It is guaranteed the answer is unique.

Example 1:
```
Input: "abbaca"
Output: "ca"
Explanation: 
For example, in "abbaca" we could remove "bb" since the letters 
are adjacent and equal, and this is the only possible move.  
The result of this move is that the string is "aaca", of which 
only "aa" is possible, so the final string is "ca".
```

Note:

- 1 <= S.length <= 20000
- S consists only of English lowercase letters.

Solution:
```cpp
class Solution {
public:
    string removeDuplicates(string S) {
        
    }
};
```
