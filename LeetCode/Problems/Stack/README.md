
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

## 496. Next Greater Element I

You are given two arrays (without duplicates) nums1 and nums2 where nums1’s elements are subset of nums2. Find all the next greater numbers for nums1's elements in the corresponding places of nums2.

The Next Greater Number of a number x in nums1 is the first greater number to its right in nums2. If it does not exist, output -1 for this number.

Example 1:
```
Input: nums1 = [4,1,2], nums2 = [1,3,4,2].
Output: [-1,3,-1]
Explanation:
    For number 4 in the first array, you cannot find the next greater 
number for it in the second array, so output -1.
    For number 1 in the first array, the next greater number for it 
in the second array is 3.
    For number 2 in the first array, there is no next greater number
for it in the second array, so output -1.
```

Example 2:
```
Input: nums1 = [2,4], nums2 = [1,2,3,4].
Output: [3,-1]
Explanation:
    For number 2 in the first array, the next greater 
number for it in the second array is 3.
    For number 4 in the first array, there is no next 
greater number for it in the second array, so output -1.
```
Note:
- All elements in nums1 and nums2 are unique.
- The length of both nums1 and nums2 would not exceed 1000.

Solution:
```cpp
class Solution {
public:
    vector<int> nextGreaterElement(vector<int>& nums1, vector<int>& nums2) {
        
    }
};
```

## 682. Baseball Game

You're now a baseball game point recorder.

Given a list of strings, each string can be one of the 4 following types:

- Integer (one round's score): Directly represents the number of points you get in this round.
- "+" (one round's score): Represents that the points you get in this round are the sum of the last two valid round's points.
- "D" (one round's score): Represents that the points you get in this round are the doubled data of the last valid round's points.
- "C" (an operation, which isn't a round's score): Represents the last valid round's points you get were invalid and should be removed.

Each round's operation is permanent and could have an impact on the round before and the round after.

You need to return the sum of the points you could get in all the rounds.

Example 1:
```
Input: ["5","2","C","D","+"]
Output: 30
Explanation: 
Round 1: You could get 5 points. The sum is: 5.
Round 2: You could get 2 points. The sum is: 7.
Operation 1: The round 2's data was invalid. The sum is: 5.  
Round 3: You could get 10 points (the round 2's data has been removed). The sum is: 15.
Round 4: You could get 5 + 10 = 15 points. The sum is: 30.
```
Example 2:
```
Input: ["5","-2","4","C","D","9","+","+"]
Output: 27
Explanation: 
Round 1: You could get 5 points. The sum is: 5.
Round 2: You could get -2 points. The sum is: 3.
Round 3: You could get 4 points. The sum is: 7.
Operation 1: The round 3's data is invalid. The sum is: 3.  
Round 4: You could get -4 points (the round 3's data has been removed). The sum is: -1.
Round 5: You could get 9 points. The sum is: 8.
Round 6: You could get -4 + 9 = 5 points. The sum is 13.
Round 7: You could get 9 + 5 = 14 points. The sum is 27.
```
Note:
- The size of the input list will be between 1 and 1000.
- Every integer represented in the list will be between -30000 and 30000.

Solution:
```cpp
class Solution {
public:
    int calPoints(vector<string>& ops) {
        
    }
};
```

## 232. Implement Queue using Stacks
 
Implement the following operations of a queue using stacks.

- push(x) -- Push element x to the back of queue.
- pop() -- Removes the element from in front of queue.
- peek() -- Get the front element.
- empty() -- Return whether the queue is empty.

Example:
```
MyQueue queue = new MyQueue();

queue.push(1);
queue.push(2);  
queue.peek();  // returns 1
queue.pop();   // returns 1
queue.empty(); // returns false
```
Notes:

- You must use only standard operations of a stack -- which means only push to top, peek/pop from top, size, and is empty operations are valid.
- Depending on your language, stack may not be supported natively. You may simulate a stack by using a list or deque (double-ended queue), as long as you use only standard operations of a stack.
- You may assume that all operations are valid (for example, no pop or peek operations will be called on an empty queue).

Solution:
```cpp
class MyQueue {
public:
    /** Initialize your data structure here. */
    MyQueue() {
        
    }
    
    /** Push element x to the back of queue. */
    void push(int x) {
        
    }
    
    /** Removes the element from in front of queue and returns that element. */
    int pop() {
        
    }
    
    /** Get the front element. */
    int peek() {
        
    }
    
    /** Returns whether the queue is empty. */
    bool empty() {
        
    }
};

/**
 * Your MyQueue object will be instantiated and called as such:
 * MyQueue* obj = new MyQueue();
 * obj->push(x);
 * int param_2 = obj->pop();
 * int param_3 = obj->peek();
 * bool param_4 = obj->empty();
 */
```
