# Linked List

## 206.Reverse Linked List

Reverse a singly linked list.

**Example:**

```
Input: 1->2->3->4->5->NULL
Output: 5->4->3->2->1->NULL
```

**Follow up:**

A linked list can be reversed either iteratively or recursively. Could you implement both?

**Solution:**
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
    ListNode* reverseList(ListNode* head) {
    }
};
```

## 21. Merge Two Sorted Lists

Merge two sorted linked lists and return it as a new sorted list. The new list should be made by 
splicing together the nodes of the first two lists.

**Example:**

```
Input: 1->2->4, 1->3->4
Output: 1->1->2->3->4->4
```

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
    ListNode* mergeTwoLists(ListNode* l1, ListNode* l2) {
    }
};
```

## 83. Remove Duplicates from Sorted List

Given a sorted linked list, delete all duplicates such that each element appear only once.

**Example 1:**
```
Input: 1->1->2
Output: 1->2
```

**Example 2:**
```
Input: 1->1->2->3->3
Output: 1->2->3
```

## 141. Linked List Cycle
Given a linked list, determine if it has a cycle in it.

To represent a cycle in the given linked list, we use an integer ```pos``` which represents the position 
(0-indexed) in the linked list where tail connects to. If ```pos``` is ```-1```, then there is no cycle 
in the linked list.

**Example 1:**
```
Input: head = [3,2,0,-4], pos = 1
Output: true
Explanation: There is a cycle in the linked list, where tail connects to the second node.
```
 
![](https://assets.leetcode.com/uploads/2018/12/07/circularlinkedlist.png)
 
**Example 2:**
```
Input: head = [1,2], pos = 0
Output: true
Explanation: There is a cycle in the linked list, where tail connects to the first node.
```

![](https://assets.leetcode.com/uploads/2018/12/07/circularlinkedlist_test2.png)

**Example 3:**
```
Input: head = [1], pos = -1
Output: false
Explanation: There is no cycle in the linked list.
```

![](https://assets.leetcode.com/uploads/2018/12/07/circularlinkedlist_test3.png)

**Follow up:**
Can you solve it using O(1) (i.e. constant) memory?

**Solution:**
```cpp
/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     ListNode *next;
 *     ListNode(int x) : val(x), next(NULL) {}
 * };
 */
class Solution {
public:
    bool hasCycle(ListNode *head) {        
    }
};
```

## 160. Intersection of Two Linked Lists

Write a program to find the node at which the intersection of two singly linked lists begins.

For example, the following two linked lists:

![](https://assets.leetcode.com/uploads/2018/12/13/160_statement.png)

begin to intersect at node c1.

**Example 1:**

![](https://assets.leetcode.com/uploads/2020/06/29/160_example_1_1.png)

```
Input: intersectVal = 8, listA = [4,1,8,4,5], listB = [5,6,1,8,4,5], skipA = 2, skipB = 3
Output: Reference of the node with value = 8
Input Explanation: The intersected node's value is 8 (note that this must not be 0 if the two lists 
intersect). From the head of A, it reads as [4,1,8,4,5]. From the head of B, it reads as [5,6,1,8,4,5].
There are 2 nodes before the intersected node in A; There are 3 nodes before the intersected node in B.
```

**Example 2:**

![](https://assets.leetcode.com/uploads/2020/06/29/160_example_2.png)

```
Input: intersectVal = 2, listA = [1,9,1,2,4], listB = [3,2,4], skipA = 3, skipB = 1
Output: Reference of the node with value = 2
Input Explanation: The intersected node's value is 2 (note that this must not be 0 if the two lists 
intersect). From the head of A, it reads as [1,9,1,2,4]. From the head of B, it reads as [3,2,4]. 
There are 3 nodes before the intersected node in A; There are 1 node before the intersected node in B.
```

**Example 3:**

![](https://assets.leetcode.com/uploads/2018/12/13/160_example_3.png)

```
Input: intersectVal = 0, listA = [2,6,4], listB = [1,5], skipA = 3, skipB = 2
Output: null
Input Explanation: From the head of A, it reads as [2,6,4]. From the head of B, it reads as [1,5]. 
Since the two lists do not intersect, intersectVal must be 0, while skipA and skipB can be arbitrary values.
Explanation: The two lists do not intersect, so return null.
```

**Notes:**
- If the two linked lists have no intersection at all, return null.
- The linked lists must retain their original structure after the function returns.
- You may assume there are no cycles anywhere in the entire linked structure.
- Each value on each linked list is in the range [1, 10^9].
- Your code should preferably run in O(n) time and use only O(1) memory.

## 234. Palindrome Linked List

Given a singly linked list, determine if it is a palindrome.

**Example 1:**
```
Input: 1->2
Output: false
```

**Example 2:**
```
Input: 1->2->2->1
Output: true
```

**Follow up:**
Could you do it in O(n) time and O(1) space?

## 203. Remove Linked List Elements

Remove all elements from a linked list of integers that have value val.

**Example:**

```
Input:  1->2->6->3->4->5->6, val = 6
Output: 1->2->3->4->5
```

## 426. Convert Binary Search Tree to Sorted Doubly Linked List

Convert a **Binary Search Tree** to a sorted **Circular Doubly-Linked List** in place.

You can think of the left and right pointers as synonymous to the predecessor and successor 
pointers in a doubly-linked list. For a circular doubly linked list, the predecessor of the 
first element is the last element, and the successor of the last element is the first element.

We want to do the transformation **in place**. After the transformation, the left pointer of the 
tree node should point to its predecessor, and the right pointer should point to its successor. 
You should return the pointer to the smallest element of the linked list.

**Example 1:**

![](https://assets.leetcode.com/uploads/2018/10/12/bstdlloriginalbst.png)

```
Input: root = [4,2,5,1,3]
```

![](https://assets.leetcode.com/uploads/2018/10/12/bstdllreturndll.png)

```
Output: [1,2,3,4,5]

Explanation: The figure below shows the transformed BST. The solid line indicates the successor 
relationship, while the dashed line means the predecessor relationship.
```

![](https://assets.leetcode.com/uploads/2018/10/12/bstdllreturnbst.png)

**Example 2:**
```
Input: root = [2,1,3]
Output: [1,2,3]
```

**Example 3:**
```
Input: root = []
Output: []
Explanation: Input is an empty tree. Output is also an empty Linked List.
```

**Example 4:**
```
Input: root = [1]
Output: [1]
```

**Constraints:**
- -1000 <= Node.val <= 1000
- Node.left.val < Node.val < Node.right.val
- All values of Node.val are unique.
- 0 <= Number of Nodes <= 2000

**Solution:**
```cpp
/*
// Definition for a Node.
class Node {
public:
    int val;
    Node* left;
    Node* right;

    Node() {}

    Node(int _val) {
        val = _val;
        left = NULL;
        right = NULL;
    }

    Node(int _val, Node* _left, Node* _right) {
        val = _val;
        left = _left;
        right = _right;
    }
};
*/

class Solution {
public:
    Node* treeToDoublyList(Node* root) {
        
    }
};
```

## 369. Plus One Linked List
Given a non-negative integer represented as **non-empty** a singly linked list of digits, plus one to the integer.

You may assume the integer do not contain any leading zero, except the number 0 itself.

The digits are stored such that the most significant digit is at the head of the list.

**Example :**
```
Input: [1,2,3]
Output: [1,2,4]
```

**Solution:**
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
    ListNode* plusOne(ListNode* head) {
        
    }
};
```

## 1019. Next Greater Node In Linked List


We are given a linked list with ```head``` as the first node.  Let's number the nodes in the list: 
```node_1, node_2, node_3, ...``` etc.

Each node may have a next larger **value**: for ```node_i, next_larger(node_i)``` is the ```node_j.val```
such that ```j > i```, ```node_j.val > node_i.val```, and ```j``` is the smallest possible choice.  If 
such a ```j``` does not exist, the next larger value is ```0```.

Return an array of integers ```answer```, where ```answer[i] = next_larger(node_{i+1})```.

Note that in the example **inputs** (not outputs) below, arrays such as ```[2,1,5]``` represent the 
serialization of a linked list with a head node value of 2, second node value of 1, and third node value of 5.

**Example 1:**
```
Input: [2,1,5]
Output: [5,5,0]
```

**Example 2:***
```
Input: [2,7,4,3,5]
Output: [7,0,5,5,0]
```

**Example 3:**
```
Input: [1,7,5,1,9,2,5,1]
Output: [7,9,9,9,0,5,0,0]
```

**Note:**

- ```1 <= node.val <= 10^9``` for each node in the linked list.
- The given list has length in the range ```[0, 10000]```.

**Solution:**
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

## 817. Linked List Components

We are given ```head```, the head node of a linked list containing **unique integer values**.

We are also given the list ```G```, a subset of the values in the linked list.

Return the number of connected components in ```G```, where two values are connected if they appear consecutively 
in the linked list.

**Example 1:**
```
Input: 
head: 0->1->2->3
G = [0, 1, 3]
Output: 2
Explanation: 
0 and 1 are connected, so [0, 1] and [3] are the two connected components.
```

**Example 2:**
```
Input: 
head: 0->1->2->3->4
G = [0, 3, 1, 4]
Output: 2
Explanation: 
0 and 1 are connected, 3 and 4 are connected, so [0, 1] and [3, 4] are the two connected components.
```

**Note:**

- If N is the length of the linked list given by ```head```, ```1 <= N <= 10000```.
- The value of each node in the linked list will be in the range ```[0, N - 1]```.
- ```1 <= G.length <= 10000.```
- ```G``` is a subset of all values in the linked list.

**Solution:**
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
    int numComponents(ListNode* head, vector<int>& G) {
        
    }
};
```

## 328. Odd Even Linked List

Given a singly linked list, group all odd nodes together followed by the even nodes. Please note here we are talking about the node number and not the value in the nodes.

You should try to do it in place. The program should run in O(1) space complexity and O(nodes) time complexity.

Example 1:
```
Input: 1->2->3->4->5->NULL
Output: 1->3->5->2->4->NULL
```

Example 2:
```
Input: 2->1->3->5->6->4->7->NULL
Output: 2->3->6->7->1->5->4->NULL
```

**Constraints:**

- The relative order inside both the even and odd groups should remain as it was in the input.
- The first node is considered odd, the second node even and so on ...
- The length of the linked list is between ```[0, 10^4]```.

**Solution:**
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
    void printList(ListNode* cur_node)
    {
    }
};
```

## 445. Add Two Numbers II

You are given two **non-empty** linked lists representing two non-negative integers. The most significant digit comes first and each of their nodes contain a single digit. Add the two numbers and return it as a linked list.

You may assume the two numbers do not contain any leading zero, except the number 0 itself.

**Follow up:**
What if you cannot modify the input lists? In other words, reversing the lists is not allowed.

**Example:**
```
Input: (7 -> 2 -> 4 -> 3) + (5 -> 6 -> 4)
Output: 7 -> 8 -> 0 -> 7
```

**Solution:**
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
    ListNode* addTwoNumbers(ListNode* l1, ListNode* l2) {
        
    }
};
```

## 430. Flatten a Multilevel Doubly Linked List

You are given a doubly linked list which in addition to the next and previous pointers, it could have a child pointer, which may or may not point to a separate doubly linked list. These child lists may have one or more children of their own, and so on, to produce a multilevel data structure, as shown in the example below.

Flatten the list so that all the nodes appear in a single-level, doubly linked list. You are given the head of the first level of the list.

 **Example 1:**
 
```
Input: head = [1,2,3,4,5,6,null,null,null,7,8,9,10,null,null,11,12]
Output: [1,2,3,7,8,11,12,9,10,4,5,6]
Explanation:

The multilevel linked list in the input is as follows:
```
 
![](https://assets.leetcode.com/uploads/2018/10/12/multilevellinkedlist.png)
 
```
After flattening the multilevel linked list it becomes:
```
 
![](https://assets.leetcode.com/uploads/2018/10/12/multilevellinkedlistflattened.png)
 
**Example 2:**
```
Input: head = [1,2,null,3]
Output: [1,3,2]
Explanation:

The input multilevel linked list is as follows:

  1---2---NULL
  |
  3---NULL
```

**Example 3:**
```
Input: head = []
Output: []
```

**How multilevel linked list is represented in test case:**

We use the multilevel linked list from **Example 1** above:
```
 1---2---3---4---5---6--NULL
         |
         7---8---9---10--NULL
             |
             11--12--NULL
```

The serialization of each level is as follows:
```
[1,2,3,4,5,6,null]
[7,8,9,10,null]
[11,12,null]
```

To serialize all levels together we will add nulls in each level to signify no node connects to the upper 
node of the previous level. The serialization becomes:
```
[1,2,3,4,5,6,null]
[null,null,7,8,9,10,null]
[null,11,12,null]
```
Merging the serialization of each level and removing trailing nulls we obtain:
```
[1,2,3,4,5,6,null,null,null,7,8,9,10,null,null,11,12]
```

**Constraints:**
- Number of Nodes will not exceed 1000.
- ```1 <= Node.val <= 10^5```


## 725. Split Linked List in Parts

Given a (singly) linked list with head node ```root```, write a function to split the linked list into ```k``` consecutive linked list "parts".

The length of each part should be as equal as possible: no two parts should have a size differing by more than 1. This may lead to some parts being null.

The parts should be in order of occurrence in the input list, and parts occurring earlier should always have a size greater than or equal parts occurring later.

Return a List of ListNode's representing the linked list parts that are formed.

Examples 1->2->3->4, k = 5 // 5 equal parts [ [1], [2], [3], [4], null ]

**Example 1:**

```
Input:
root = [1, 2, 3], k = 5
Output: [[1],[2],[3],[],[]]
Explanation:
The input and each element of the output are ListNodes, not arrays.
For example, the input root has root.val = 1, root.next.val = 2, \root.next.next.val = 3, 
and root.next.next.next = null. The first element output[0] has output[0].val = 1, 
output[0].next = null. The last element output[4] is null, but it's string representation 
as a ListNode is [].
```

**Example 2:**
```
Input: 
root = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10], k = 3
Output: [[1, 2, 3, 4], [5, 6, 7], [8, 9, 10]]
Explanation:
The input has been split into consecutive parts with size difference at most 1, and earlier 
parts are a larger size than the later parts.
```

**Note:**

- The length of ```root``` will be in the range ```[0, 1000]```.
- Each value of a node in the input will be an integer in the range ```[0, 999]```.
- ```k``` will be an integer in the range ```[1, 50]```.

**Solution:**

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
    vector<ListNode*> splitListToParts(ListNode* root, int k) {
        
    }
};
```

## 24.Swap Nodes in Pairs

Given a linked list, swap every two adjacent nodes and return its head.

You may not modify the values in the list's nodes, only nodes itself may be changed.

Example:
```
Given 1->2->3->4, you should return the list as 2->1->4->3.
```

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
    ListNode* swapPairs(ListNode* head) {
        
    }
};
```

## 109. Convert Sorted List to Binary Search Tree

Given a singly linked list where elements are sorted in ascending order, convert it to a height balanced BST.

For this problem, a height-balanced binary tree is defined as a binary tree in which the depth of the two subtrees of every node never differ by more than 1.

**Example:**
```
Given the sorted linked list: [-10,-3,0,5,9],

One possible answer is: [0,-3,9,-10,null,5], which represents the following height balanced BST:

      0
     / \
   -3   9
   /   /
 -10  5
```

**Solution:**

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
    TreeNode* sortedListToBST(ListNode* head) {
        
    }
};
```

## 379. Design Phone Directory
Design a Phone Directory which supports the following operations:

- ```get```: Provide a number which is not assigned to anyone.
- ```check```: Check if a number is available or not.
- ```release```: Recycle or release a number.
 
 **Example:**
 ```
 // Init a phone directory containing a total of 3 numbers: 0, 1, and 2.
PhoneDirectory directory = new PhoneDirectory(3);

// It can return any available phone number. Here we assume it returns 0.
directory.get();

// Assume it returns 1.
directory.get();

// The number 2 is available, so return true.
directory.check(2);

// It returns 2, the only number that is left.
directory.get();

// The number 2 is no longer available, so return false.
directory.check(2);

// Release number 2 back to the pool.
directory.release(2);

// Number 2 is available again, return true.
directory.check(2);
```

**Constraints:**
- ```1 <= maxNumbers <= 10^4```
- ```0 <= number < maxNumbers```
- The total number of call of the methods is between ```[0 - 20000]```

**Solution:**
```cpp
class PhoneDirectory {
public:
    /** Initialize your data structure here
        @param maxNumbers - The maximum numbers that can be stored in the phone directory. */
    PhoneDirectory(int maxNumbers) {
        
    }
    
    /** Provide a number which is not assigned to anyone.
        @return - Return an available number. Return -1 if none is available. */
    int get() {
        
    }
    
    /** Check if a number is available or not. */
    bool check(int number) {
        
    }
    
    /** Recycle or release a number. */
    void release(int number) {
        
    }
};

/**
 * Your PhoneDirectory object will be instantiated and called as such:
 * PhoneDirectory* obj = new PhoneDirectory(maxNumbers);
 * int param_1 = obj->get();
 * bool param_2 = obj->check(number);
 * obj->release(number);
 */
```

## 148. Sort List
Sort a linked list in O(n log n) time using constant space complexity.

**Example 1:**
```
Input: 4->2->1->3
Output: 1->2->3->4
```

**Example 2:**
```
Input: -1->5->3->4->0
Output: -1->0->3->4->5
```

**Solution:**
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
    ListNode* sortList(ListNode* head) {
        
    }
};
```
