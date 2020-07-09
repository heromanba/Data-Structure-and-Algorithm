
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

## 844. Backspace String Compare

Given two strings S and T, return if they are equal when both are typed into empty text editors. # means a backspace character.

Note that after backspacing an empty text, the text will continue empty.

Example 1:
```
Input: S = "ab#c", T = "ad#c"
Output: true
Explanation: Both S and T become "ac".
```

Example 2:
```
Input: S = "ab##", T = "c#d#"
Output: true
Explanation: Both S and T become "".
```

Example 3:
```
Input: S = "a##c", T = "#a#c"
Output: true
Explanation: Both S and T become "c".
```

Example 4:
```
Input: S = "a#c", T = "b"
Output: false
Explanation: S becomes "c" while T becomes "b".
```
Note:

- 1 <= S.length <= 200
- 1 <= T.length <= 200
- S and T only contain lowercase letters and '#' characters.

Follow up:

Can you solve it in O(N) time and O(1) space?

Solution:
```cpp
class Solution {
public:
    bool backspaceCompare(string S, string T) {
        
    }
};
```

## 225. Implement Stack using Queues

Implement the following operations of a stack using queues.

- push(x) -- Push element x onto stack.
- pop() -- Removes the element on top of the stack.
- top() -- Get the top element.
- empty() -- Return whether the stack is empty.

Example:
```
MyStack stack = new MyStack();

stack.push(1);
stack.push(2);  
stack.top();   // returns 2
stack.pop();   // returns 2
stack.empty(); // returns false
```

Notes:

- You must use only standard operations of a queue -- which means only push to back, peek/pop from front, size, and is empty operations are valid.
- Depending on your language, queue may not be supported natively. You may simulate a queue by using a list or deque (double-ended queue), as long as you use only standard operations of a queue.
- You may assume that all operations are valid (for example, no pop or top operations will be called on an empty stack).

Solution:
```cpp
class MyStack {
public:
    /** Initialize your data structure here. */
    MyStack() {
        
    }
    
    /** Push element x onto stack. */
    void push(int x) {
        
    }
    
    /** Removes the element on top of the stack and returns that element. */
    int pop() {
        
    }
    
    /** Get the top element. */
    int top() {
        
    }
    
    /** Returns whether the stack is empty. */
    bool empty() {
        
    }
};

/**
 * Your MyStack object will be instantiated and called as such:
 * MyStack* obj = new MyStack();
 * obj->push(x);
 * int param_2 = obj->pop();
 * int param_3 = obj->top();
 * bool param_4 = obj->empty();
 */
```

## 155. Min Stack

Design a stack that supports push, pop, top, and retrieving the minimum element in constant time.

- push(x) -- Push element x onto stack.
- pop() -- Removes the element on top of the stack.
- top() -- Get the top element.
- getMin() -- Retrieve the minimum element in the stack.
 
Example 1:
```
Input
["MinStack","push","push","push","getMin","pop","top","getMin"]
[[],[-2],[0],[-3],[],[],[],[]]

Output
[null,null,null,null,-3,null,0,-2]

Explanation
MinStack minStack = new MinStack();
minStack.push(-2);
minStack.push(0);
minStack.push(-3);
minStack.getMin(); // return -3
minStack.pop();
minStack.top();    // return 0
minStack.getMin(); // return -2
```

Constraints:

- Methods pop, top and getMin operations will always be called on non-empty stacks.

Solution:
```cpp
class MinStack {
public:
    /** initialize your data structure here. */
    MinStack() {
        
    }
    
    void push(int x) {
        
    }
    
    void pop() {
        
    }
    
    int top() {
        
    }
    
    int getMin() {
        
    }
};

/**
 * Your MinStack object will be instantiated and called as such:
 * MinStack* obj = new MinStack();
 * obj->push(x);
 * obj->pop();
 * int param_3 = obj->top();
 * int param_4 = obj->getMin();
 */
```

## 20. Valid Parentheses

Given a string containing just the characters '(', ')', '{', '}', '[' and ']', determine if the input string is valid.

An input string is valid if:

Open brackets must be closed by the same type of brackets.
Open brackets must be closed in the correct order.
Note that an empty string is also considered valid.

Example 1:
```
Input: "()"
Output: true
```

Example 2:
```
Input: "()[]{}"
Output: true
```

Example 3:
```
Input: "(]"
Output: false
```

Example 4:
```
Input: "([)]"
Output: false
```
Example 5:
```
Input: "{[]}"
Output: true
```

Solution:
```cpp
class Solution {
public:
    bool isValid(string s) {
        
    }
};
```

## 1381. Design a Stack With Increment Operation

Design a stack which supports the following operations.

Implement the CustomStack class:

- CustomStack(int maxSize) Initializes the object with maxSize which is the maximum number of elements in the stack or do nothing if the stack reached the maxSize.
- void push(int x) Adds x to the top of the stack if the stack hasn't reached the maxSize.
- int pop() Pops and returns the top of stack or -1 if the stack is empty.
- void inc(int k, int val) Increments the bottom k elements of the stack by val. If there are less than k elements in the stack, just increment all the elements in the stack.
 
Example 1:
```
Input
["CustomStack","push","push","pop","push",
 "push","push","increment","increment","pop","pop","pop","pop"]
 
[[3],[1],[2],[],[2],[3],[4],[5,100],[2,100],[],[],[],[]]

Output
[null,null,null,2,null,null,null,null,null,103,202,201,-1]

Explanation
CustomStack customStack = new CustomStack(3); // Stack is Empty []
customStack.push(1);                          // stack becomes [1]
customStack.push(2);                          // stack becomes [1, 2]
customStack.pop();    // return 2 --> Return top of the stack 2, stack becomes [1]
customStack.push(2);    // stack becomes [1, 2]
customStack.push(3);    // stack becomes [1, 2, 3]
customStack.push(4);    // stack still [1, 2, 3], Don't add another elements as size is 4
customStack.increment(5, 100);    // stack becomes [101, 102, 103]
customStack.increment(2, 100);    // stack becomes [201, 202, 103]
customStack.pop();    // return 103 --> Return top of the stack 103, stack becomes [201, 202]
customStack.pop();    // return 202 --> Return top of the stack 102, stack becomes [201]
customStack.pop();    // return 201 --> Return top of the stack 101, stack becomes []
customStack.pop();    // return -1 --> Stack is empty return -1.
```

Constraints:

- 1 <= maxSize <= 1000
- 1 <= x <= 1000
- 1 <= k <= 1000
- 0 <= val <= 100
- At most 1000 calls will be made to each method of increment, push and pop each separately.

Solution:
```cpp
class CustomStack {
public:
    CustomStack(int maxSize) {
        
    }
    
    void push(int x) {
        
    }
    
    int pop() {
        
    }
    
    void increment(int k, int val) {
        
    }
};

/**
 * Your CustomStack object will be instantiated and called as such:
 * CustomStack* obj = new CustomStack(maxSize);
 * obj->push(x);
 * int param_2 = obj->pop();
 * obj->increment(k,val);
 */
```

## 921. Minimum Add to Make Parentheses Valid

Given a string S of '(' and ')' parentheses, we add the minimum number of parentheses ( '(' or ')', and in any positions ) so that the resulting parentheses string is valid.

Formally, a parentheses string is valid if and only if:

- It is the empty string, or
- It can be written as AB (A concatenated with B), where A and B are valid strings, or
- It can be written as (A), where A is a valid string.

Given a parentheses string, return the minimum number of parentheses we must add to make the resulting string valid.

Example 1:
```
Input: "())"
Output: 1
```

Example 2:
```
Input: "((("
Output: 3
```
Example 3:
```
Input: "()"
Output: 0
```
Example 4:
```
Input: "()))(("
Output: 4
```

Note:

- S.length <= 1000
- S only consists of '(' and ')' characters.

Solution:
```cpp
class Solution {
public:
    int minAddToMakeValid(string S) {
        
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
There are two possible trees.  The first has non-leaf node sum 36, 
and the second has non-leaf node sum 32.

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

## 739. Daily Temperatures

Given a list of daily temperatures T, return a list such that, for each day in the input, tells you how many days you would have to wait until a warmer temperature. If there is no future day for which this is possible, put 0 instead.

For example, given the list of temperatures T = [73, 74, 75, 71, 69, 72, 76, 73], your output should be [1, 1, 4, 2, 1, 1, 0, 0].

Note: The length of temperatures will be in the range [1, 30000]. Each temperature will be an integer in the range [30, 100].

Solution:
```cpp
class Solution {
public:
    vector<int> dailyTemperatures(vector<int>& T) {
        
    }
};
```

## 94. Binary Tree Inorder Traversal

Given a binary tree, return the inorder traversal of its nodes' values.

Example:
```
Input: [1,null,2,3]
   1
    \
     2
    /
   3

Output: [1,3,2]
```
Follow up: Recursive solution is trivial, could you do it iteratively?

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
    vector<int> inorderTraversal(TreeNode* root) {
        
    }
};
```

## 1249. Minimum Remove to Make Valid Parentheses

Given a string s of '(' , ')' and lowercase English characters. 

Your task is to remove the minimum number of parentheses ( '(' or ')', in any positions ) so that the resulting parentheses string is valid and return any valid string.

Formally, a parentheses string is valid if and only if:

- It is the empty string, contains only lowercase characters, or
- It can be written as AB (A concatenated with B), where A and B are valid strings, or
- It can be written as (A), where A is a valid string.
 
Example 1:
```
Input: s = "lee(t(c)o)de)"
Output: "lee(t(c)o)de"
Explanation: "lee(t(co)de)" , "lee(t(c)ode)" would also be accepted.
```

Example 2:
```
Input: s = "a)b(c)d"
Output: "ab(c)d"
```

Example 3:
```
Input: s = "))(("
Output: ""
Explanation: An empty string is also valid.
```

Example 4:
```
Input: s = "(a(b(c)d)"
Output: "a(b(c)d)"
```

Constraints:

- 1 <= s.length <= 10^5
- s[i] is one of  '(' , ')' and lowercase English letters.

Solution:
```cpp
class Solution {
public:
    string minRemoveToMakeValid(string s) {
        
    }
};
```

## 946. Validate Stack Sequences

Given two sequences pushed and popped with distinct values, return true if and only if this could have been the result of a sequence of push and pop operations on an initially empty stack.

Example 1:
```
Input: pushed = [1,2,3,4,5], popped = [4,5,3,2,1]
Output: true
Explanation: We might do the following sequence:
push(1), push(2), push(3), push(4), pop() -> 4,
push(5), pop() -> 5, pop() -> 3, pop() -> 2, pop() -> 1
```

Example 2:
```
Input: pushed = [1,2,3,4,5], popped = [4,3,5,1,2]
Output: false
Explanation: 1 cannot be popped before 2.
``` 

Note:

- 0 <= pushed.length == popped.length <= 1000
- 0 <= pushed[i], popped[i] < 1000
- pushed is a permutation of popped.
- pushed and popped have distinct values.

Solution:

```cpp
class Solution {
public:
    bool validateStackSequences(vector<int>& pushed, vector<int>& popped) {
        
    }
};
```

## 1190. Reverse Substrings Between Each Pair of Parentheses

You are given a string s that consists of lower case English letters and brackets. 

Reverse the strings in each pair of matching parentheses, starting from the innermost one.

Your result should not contain any brackets.

Example 1:
```
Input: s = "(abcd)"
Output: "dcba"
```
Example 2:
```
Input: s = "(u(love)i)"
Output: "iloveu"
Explanation: The substring "love" is reversed first, then the whole string is reversed.
```
Example 3:
```
Input: s = "(ed(et(oc))el)"
Output: "leetcode"
Explanation: First, we reverse the substring "oc", then "etco", and finally, the whole 
string.
```
Example 4:
```
Input: s = "a(bcdefghijkl(mno)p)q"
Output: "apmnolkjihgfedcbq"
```

Constraints:

- 0 <= s.length <= 2000
- s only contains lower case English characters and parentheses.
- It's guaranteed that all parentheses are balanced.

Solution:
```cpp
class Solution {
public:
    string reverseParentheses(string s) {
        
    }
};
```

## 856. Score of Parentheses

Given a balanced parentheses string S, compute the score of the string based on the following rule:

- () has score 1
- AB has score A + B, where A and B are balanced parentheses strings.
- (A) has score 2 * A, where A is a balanced parentheses string.
 

Example 1:
```
Input: "()"
Output: 1
```
Example 2:
```
Input: "(())"
Output: 2
```
Example 3:
```
Input: "()()"
Output: 2
```
Example 4:
```
Input: "(()(()))"
Output: 6
```

Note:

- S is a balanced parentheses string, containing only ( and ).
- 2 <= S.length <= 50

Solution:
```cpp
class Solution {
public:
    int scoreOfParentheses(string S) {
        
    }
};
```

## 901. Online Stock Span

Write a class StockSpanner which collects daily price quotes for some stock, and returns the span of that stock's price for the current day.

The span of the stock's price today is defined as the maximum number of consecutive days (starting from today and going backwards) for which the price of the stock was less than or equal to today's price.

For example, if the price of a stock over the next 7 days were [100, 80, 60, 70, 60, 75, 85], then the stock spans would be [1, 1, 1, 2, 1, 4, 6].

 

Example 1:
```
Input: ["StockSpanner","next","next","next","next","next","next","next"], 
    [[],[100],[80],[60],[70],[60],[75],[85]]
Output: [null,1,1,1,2,1,4,6]
Explanation: 
First, S = StockSpanner() is initialized.  Then:
S.next(100) is called and returns 1,
S.next(80) is called and returns 1,
S.next(60) is called and returns 1,
S.next(70) is called and returns 2,
S.next(60) is called and returns 1,
S.next(75) is called and returns 4,
S.next(85) is called and returns 6.

Note that (for example) S.next(75) returned 4, because the last 4 prices
(including today's price of 75) were less than or equal to today's price.
```

Note:

- Calls to StockSpanner.next(int price) will have 1 <= price <= 10^5.
- There will be at most 10000 calls to StockSpanner.next per test case.
- There will be at most 150000 calls to StockSpanner.next across all test cases.
- The total time limit for this problem has been reduced by 75% for C++, and 50% for all other languages.

Solution:
```cpp
class StockSpanner {
public:
    StockSpanner() {
        
    }
    
    int next(int price) {
        
    }
};

/**
 * Your StockSpanner object will be instantiated and called as such:
 * StockSpanner* obj = new StockSpanner();
 * int param_1 = obj->next(price);
 */
```

## 1019. Next Greater Node In Linked List

We are given a linked list with head as the first node.  Let's number the nodes in the list: node_1, node_2, node_3, ... etc.

Each node may have a next larger value: for node_i, next_larger(node_i) is the node_j.val such that j > i, node_j.val > node_i.val, and j is the smallest possible choice.  If such a j does not exist, the next larger value is 0.

Return an array of integers answer, where answer[i] = next_larger(node_{i+1}).

Note that in the example inputs (not outputs) below, arrays such as [2,1,5] represent the serialization of a linked list with a head node value of 2, second node value of 1, and third node value of 5.

 

Example 1:
```
Input: [2,1,5]
Output: [5,5,0]
```
Example 2:
```
Input: [2,7,4,3,5]
Output: [7,0,5,5,0]
```
Example 3:
```
Input: [1,7,5,1,9,2,5,1]
Output: [7,9,9,9,0,5,0,0]
``` 

Note:

- 1 <= node.val <= 10^9 for each node in the linked list.
- The given list has length in the range [0, 10000].

Solution:
```cpp
/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     ListNode *next;
 *     ListNode() : val(0), next(nullptr) {}
 *     ListNode(int x) : val(x), next(nullptr) {}
 *     ListNode(int x, ListNode *next) : val(x), next(next) {}
 * };
 */
class Solution {
public:
    vector<int> nextLargerNodes(ListNode* head) {
        
    }
};
```

## 1209. Remove All Adjacent Duplicates in String II
 
Given a string s, a k duplicate removal consists of choosing k adjacent and equal letters from s and removing them causing the left and the right side of the deleted substring to concatenate together.

We repeatedly make k duplicate removals on s until we no longer can.

Return the final string after all such duplicate removals have been made.

It is guaranteed that the answer is unique.

Example 1:
```
Input: s = "abcd", k = 2
Output: "abcd"
Explanation: There's nothing to delete.
```
Example 2:
```
Input: s = "deeedbbcccbdaa", k = 3
Output: "aa"
Explanation: 
First delete "eee" and "ccc", get "ddbbbdaa"
Then delete "bbb", get "dddaa"
Finally delete "ddd", get "aa"
```
Example 3:
```
Input: s = "pbbcggttciiippooaais", k = 2
Output: "ps"
``` 

Constraints:

- 1 <= s.length <= 10^5
- 2 <= k <= 10^4
- s only contains lower case English letters.

Solution:
```cpp
class Solution {
public:
    string removeDuplicates(string s, int k) {
        
    }
};
```

## 503. Next Greater Element II

Given a circular array (the next element of the last element is the first element of the array), print the Next Greater Number for every element. The Next Greater Number of a number x is the first greater number to its traversing-order next in the array, which means you could search circularly to find its next greater number. If it doesn't exist, output -1 for this number.

Example 1:
```
Input: [1,2,1]
Output: [2,-1,2]
Explanation: The first 1's next greater number is 2; 
The number 2 can't find next greater number; 
The second 1's next greater number needs to search circularly, which is also 2.
```
Note: The length of given array won't exceed 10000.

Solution:
```cpp
class Solution {
public:
    vector<int> nextGreaterElements(vector<int>& nums) {
        
    }
};
```

## 173. Binary Search Tree Iterator
 
Implement an iterator over a binary search tree (BST). Your iterator will be initialized with the root node of a BST.

Calling next() will return the next smallest number in the BST.

Example:

![](https://assets.leetcode.com/uploads/2018/12/25/bst-tree.png)

```
BSTIterator iterator = new BSTIterator(root);
iterator.next();    // return 3
iterator.next();    // return 7
iterator.hasNext(); // return true
iterator.next();    // return 9
iterator.hasNext(); // return true
iterator.next();    // return 15
iterator.hasNext(); // return true
iterator.next();    // return 20
iterator.hasNext(); // return false
```

Note:

- next() and hasNext() should run in average O(1) time and uses O(h) memory, where h is the height of the tree.
- You may assume that next() call will always be valid, that is, there will be at least a next smallest number in the BST when next() is called.

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
class BSTIterator {
public:
    BSTIterator(TreeNode* root) {
        
    }
    
    /** @return the next smallest number */
    int next() {
        
    }
    
    /** @return whether we have a next smallest number */
    bool hasNext() {
        
    }
};

/**
 * Your BSTIterator object will be instantiated and called as such:
 * BSTIterator* obj = new BSTIterator(root);
 * int param_1 = obj->next();
 * bool param_2 = obj->hasNext();
 */
```

## 439. Ternary Expression Parser

Given a string representing arbitrarily nested ternary expressions, calculate the result of the expression. You can always assume that the given expression is valid and only consists of digits 0-9, ?, :, T and F (T and F represent True and False respectively).

Note:

- The length of the given string is ≤ 10000.
- Each number will contain only one digit.
- The conditional expressions group right-to-left (as usual in most languages).
- The condition will always be either T or F. That is, the condition will never be a digit.
- The result of the expression will always evaluate to either a digit 0-9, T or F.

Example 1:
```
Input: "T?2:3"

Output: "2"

Explanation: If true, then result is 2; otherwise result is 3.
```

Example 2:
```
Input: "F?1:T?4:5"

Output: "4"

Explanation: The conditional expressions group right-to-left. Using parenthesis, it is read/evaluated as:

             "(F ? 1 : (T ? 4 : 5))"                   "(F ? 1 : (T ? 4 : 5))"
          -> "(F ? 1 : 4)"                 or       -> "(T ? 4 : 5)"
          -> "4"                                    -> "4"
```

Example 3:
```
Input: "T?T?F:5:3"

Output: "F"

Explanation: The conditional expressions group right-to-left. Using parenthesis, it is read/evaluated as:

             "(T ? (T ? F : 5) : 3)"                   "(T ? (T ? F : 5) : 3)"
          -> "(T ? F : 3)"                 or       -> "(T ? F : 5)"
          -> "F"                                    -> "F"
```

Solution:
```cpp
class Solution {
public:
    string parseTernary(string expression) {
        
    }
};
```

## 144. Binary Tree Preorder Traversal

Given a binary tree, return the preorder traversal of its nodes' values.

Example:
```
Input: [1,null,2,3]
   1
    \
     2
    /
   3

Output: [1,2,3]
```

Follow up: Recursive solution is trivial, could you do it iteratively?

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
    vector<int> preorderTraversal(TreeNode* root) {
        
    }
};
```

## 1003. Check If Word Is Valid After Substitutions
 
We are given that the string "abc" is valid.

From any valid string V, we may split V into two pieces X and Y such that X + Y (X concatenated with Y) is equal to V.  (X or Y may be empty.)  Then, X + "abc" + Y is also valid.

If for example S = "abc", then examples of valid strings are: "abc", "aabcbc", "abcabc", "abcabcababcc".  Examples of invalid strings are: "abccba", "ab", "cababc", "bac".

Return true if and only if the given string S is valid.

Example 1:
```
Input: "aabcbc"
Output: true
Explanation: 
We start with the valid string "abc".
Then we can insert another "abc" between "a" and "bc", resulting in "a" + "abc" + "bc" which is "aabcbc".
```
Example 2:
```
Input: "abcabcababcc"
Output: true
Explanation: 
"abcabcabc" is valid after consecutive insertings of "abc".
Then we can insert "abc" before the last letter, resulting in "abcabcab" + "abc" + "c" which is "abcabcababcc".
```
Example 3:
```
Input: "abccba"
Output: false
```
Example 4:
```
Input: "cababc"
Output: false
```

Note:

- 1 <= S.length <= 20000
- S[i] is 'a', 'b', or 'c'

Solution:
```cpp
class Solution {
public:
    bool isValid(string S) {
        
    }
};
```

## 1410. HTML Entity Parser
 
HTML entity parser is the parser that takes HTML code as input and replace all the entities of the special characters by the characters itself.

The special characters and their entities for HTML are:

- Quotation Mark: the entity is &quot; and symbol character is ".
- Single Quote Mark: the entity is &apos; and symbol character is '.
- Ampersand: the entity is &amp; and symbol character is &.
- Greater Than Sign: the entity is &gt; and symbol character is >.
- Less Than Sign: the entity is &lt; and symbol character is <.
- Slash: the entity is &frasl; and symbol character is /.

Given the input text string to the HTML parser, you have to implement the entity parser.

Return the text after replacing the entities by the special characters.

Example 1:
```
Input: text = "&amp; is an HTML entity but &ambassador; is not."
Output: "& is an HTML entity but &ambassador; is not."
Explanation: The parser will replace the &amp; entity by &
```

Example 2:
```
Input: text = "and I quote: &quot;...&quot;"
Output: "and I quote: \"...\""
```

Example 3:
```
Input: text = "Stay home! Practice on Leetcode :)"
Output: "Stay home! Practice on Leetcode :)"
```

Example 4:
```
Input: text = "x &gt; y &amp;&amp; x &lt; y is always false"
Output: "x > y && x < y is always false"
```

Example 5:
```
Input: text = "leetcode.com&frasl;problemset&frasl;all"
Output: "leetcode.com/problemset/all"
```

Constraints:

- 1 <= text.length <= 10^5
- The string may contain any possible characters out of all the 256 ASCII characters.

Solution:
```cpp
class Solution {
public:
    string entityParser(string text) {
        
    }
};
```

## 341. Flatten Nested List Iterator

Given a nested list of integers, implement an iterator to flatten it.

Each element is either an integer, or a list -- whose elements may also be integers or other lists.

Example 1:
```
Input: [[1,1],2,[1,1]]
Output: [1,1,2,1,1]
Explanation: By calling next repeatedly until hasNext returns false, 
             the order of elements returned by next should be: [1,1,2,1,1].
```

Example 2:
```
Input: [1,[4,[6]]]
Output: [1,4,6]
Explanation: By calling next repeatedly until hasNext returns false, 
             the order of elements returned by next should be: [1,4,6].
```

Solution:
```cpp
/**
 * // This is the interface that allows for creating nested lists.
 * // You should not implement it, or speculate about its implementation
 * class NestedInteger {
 *   public:
 *     // Return true if this NestedInteger holds a single integer, rather than a nested list.
 *     bool isInteger() const;
 *
 *     // Return the single integer that this NestedInteger holds, if it holds a single integer
 *     // The result is undefined if this NestedInteger holds a nested list
 *     int getInteger() const;
 *
 *     // Return the nested list that this NestedInteger holds, if it holds a nested list
 *     // The result is undefined if this NestedInteger holds a single integer
 *     const vector<NestedInteger> &getList() const;
 * };
 */

class NestedIterator {
public:
    NestedIterator(vector<NestedInteger> &nestedList) {
        
    }
    
    int next() {
        
    }
    
    bool hasNext() {
        
    }
};

/**
 * Your NestedIterator object will be instantiated and called as such:
 * NestedIterator i(nestedList);
 * while (i.hasNext()) cout << i.next();
 */
```

## 636. Exclusive Time of Functions

On a single threaded CPU, we execute some functions.  Each function has a unique id between 0 and N-1.

We store logs in timestamp order that describe when a function is entered or exited.

Each log is a string with this format: "{function_id}:{"start" | "end"}:{timestamp}".  For example, "0:start:3" means the function with id 0 started at the beginning of timestamp 3.  "1:end:2" means the function with id 1 ended at the end of timestamp 2.

A function's exclusive time is the number of units of time spent in this function.  Note that this does not include any recursive calls to child functions.

The CPU is single threaded which means that only one function is being executed at a given time unit.

Return the exclusive time of each function, sorted by their function id.

 

Example 1:

![](https://assets.leetcode.com/uploads/2019/04/05/diag1b.png)

```
Input:
n = 2
logs = ["0:start:0","1:start:2","1:end:5","0:end:6"]
Output: [3, 4]
Explanation:
Function 0 starts at the beginning of time 0, then it executes 2 units 
of time and reaches the end of time 1.
Now function 1 starts at the beginning of time 2, executes 4 units of 
time and ends at time 5.
Function 0 is running again at the beginning of time 6, and also ends 
at the end of time 6, thus executing for 1 unit of time. 
So function 0 spends 2 + 1 = 3 units of total time executing, and 
function 1 spends 4 units of total time executing.
```

Note:

- 1 <= n <= 100
- Two functions won't start or end at the same time.
- Functions will always log when they exit.

Solution:
```cpp
class Solution {
public:
    vector<int> exclusiveTime(int n, vector<string>& logs) {
        
    }
};
```

## 394. Decode String
 
Given an encoded string, return its decoded string.

The encoding rule is: k[encoded_string], where the encoded_string inside the square brackets is being repeated exactly k times. Note that k is guaranteed to be a positive integer.

You may assume that the input string is always valid; No extra white spaces, square brackets are well-formed, etc.

Furthermore, you may assume that the original data does not contain any digits and that digits are only for those repeat numbers, k. For example, there won't be input like 3a or 2[4].

Example 1:
```
Input: s = "3[a]2[bc]"
Output: "aaabcbc"
```

Example 2:
```
Input: s = "3[a2[c]]"
Output: "accaccacc"
```

Example 3:
```
Input: s = "2[abc]3[cd]ef"
Output: "abcabccdcdcdef"
```
Example 4:
```
Input: s = "abc3[cd]xyz"
Output: "abccdcdcdxyz"
```

Solution:
```cpp
class Solution {
public:
    string decodeString(string s) {
        
    }
};
```

## 103. Binary Tree Zigzag Level Order Traversal
 
Given a binary tree, return the zigzag level order traversal of its nodes' values. (ie, from left to right, then right to left for the next level and alternate between).

For example:
Given binary tree [3,9,20,null,null,15,7],
```
    3
   / \
  9  20
    /  \
   15   7
```
return its zigzag level order traversal as:
```
[
  [3],
  [20,9],
  [15,7]
]
```
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
    vector<vector<int>> zigzagLevelOrder(TreeNode* root) {
        
    }
};
```

## 255. Verify Preorder Sequence in Binary Search Tree
 
Given an array of numbers, verify whether it is the correct preorder traversal sequence of a binary search tree.

You may assume each number in the sequence is unique.

Consider the following binary search tree: 
```
     5
    / \
   2   6
  / \
 1   3
```
Example 1:
```
Input: [5,2,6,1,3]
Output: false
```
Example 2:
```
Input: [5,2,1,3,6]
Output: true
```
Follow up:
Could you do it using only constant space complexity?

Solution:
```cpp
class Solution {
public:
    bool verifyPreorder(vector<int>& preorder) {
        
    }
};
```
