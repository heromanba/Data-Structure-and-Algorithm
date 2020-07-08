
# Tree (Medium)

## 1490. Clone N-ary Tree
Given a root of an N-ary tree, return a [deep copy](https://en.wikipedia.org/wiki/Object_copying#Deep_copy) (clone) of the tree.

Each node in the n-ary tree contains a val (int) and a list (List[Node]) of its children.
```
class Node {
    public int val;
    public List<Node> children;
}
```
Nary-Tree input serialization is represented in their level order traversal, each group of children is separated by the null value (See examples).

Follow up: Can your solution work for the [graph problem](https://leetcode.com/problems/clone-graph/)?

Example 1:

![](https://assets.leetcode.com/uploads/2018/10/12/narytreeexample.png)

```

Input: root = [1,null,3,2,4,null,5,6]
Output: [1,null,3,2,4,null,5,6]
```

Example 2:

![](https://assets.leetcode.com/uploads/2019/11/08/sample_4_964.png)

```
Input: root = [1,null,2,3,4,5,null,null,6,7,null,8,null,9,10,null,
null,11,null,12,null,13,null,null,14]

Output: [1,null,2,3,4,5,null,null,6,7,null,8,null,9,10,null,null,11,null,
12,null,13,null,null,14]
```

Constraints:

- The depth of the n-ary tree is less than or equal to 1000.
- The total number of nodes is between [0, 10^4].

Solution:

```cpp
/*
// Definition for a Node.
class Node {
public:
    int val;
    vector<Node*> children;

    Node() {}

    Node(int _val) {
        val = _val;
    }

    Node(int _val, vector<Node*> _children) {
        val = _val;
        children = _children;
    }
};
*/

class Solution {
public:
    Node* cloneTree(Node* root) {
        
    }
};
```

## 1302. Deepest Leaves Sum

Given a binary tree, return the sum of values of its deepest leaves.
 

Example 1:

![](https://assets.leetcode.com/uploads/2019/07/31/1483_ex1.png)

Input: root = [1,2,3,4,5,null,6,7,null,null,null,null,8]
Output: 15

Constraints:

- The number of nodes in the tree is between 1 and 10^4.
- The value of nodes is between 1 and 100.

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
    int deepestLeavesSum(TreeNode* root) {
        
    }
};
```

## 1379. Find a Corresponding Node of a Binary Tree in a Clone of That Tree

Given two binary trees original and cloned and given a reference to a node target in the original tree.

The cloned tree is a copy of the original tree.

Return a reference to the same node in the cloned tree.

Note that you are not allowed to change any of the two trees or the target node and the answer must be a reference to a node in the cloned tree.

Follow up: Solve the problem if repeated values on the tree are allowed.

Example 1:

![](https://assets.leetcode.com/uploads/2020/02/21/e1.png)

```
Input: tree = [7,4,3,null,null,6,19], target = 3
Output: 3
Explanation: In all examples the original and cloned trees are shown. 
The target node is a green node from the original tree. 
The answer is the yellow node from the cloned tree.
```

Example 2:

![](https://assets.leetcode.com/uploads/2020/02/21/e2.png)

```
Input: tree = [7], target =  7
Output: 7
```

Example 3:

![](https://assets.leetcode.com/uploads/2020/02/21/e3.png)

```
Input: tree = [8,null,6,null,5,null,4,null,3,null,2,null,1], target = 4
Output: 4
```

Example 4:

![](https://assets.leetcode.com/uploads/2020/02/21/e4.png)

```
Input: tree = [1,2,3,4,5,6,7,8,9,10], target = 5
Output: 5
```

Example 5:

![](https://assets.leetcode.com/uploads/2020/02/21/e5.png)

```
Input: tree = [1,2,null,3], target = 2
Output: 2
```

Constraints:

- The number of nodes in the tree is in the range [1, 10^4].
- The values of the nodes of the tree are unique.
- target node is a node from the original tree and is not null.

Solution:

```cpp
/**
 * Definition for a binary tree node.
 * struct TreeNode {
 *     int val;
 *     TreeNode *left;
 *     TreeNode *right;
 *     TreeNode(int x) : val(x), left(NULL), right(NULL) {}
 * };
 */

class Solution {
public:
    TreeNode* getTargetCopy(TreeNode* original, TreeNode* cloned, TreeNode* target) {
        
    }
};
```

## 1315. Sum of Nodes with Even-Valued Grandparent

Given a binary tree, return the sum of values of nodes with even-valued grandparent.  (A grandparent of a node is the parent of its parent, if it exists.)

If there are no nodes with an even-valued grandparent, return 0.

Example 1:

![](https://assets.leetcode.com/uploads/2019/07/24/1473_ex1.png)

```
Input: root = [6,7,8,2,7,1,3,9,null,1,4,null,null,null,5]
Output: 18
Explanation: The red nodes are the nodes with even-value grandparent while the 
blue nodes are the even-value grandparents.
```

Constraints:

- The number of nodes in the tree is between 1 and 10^4.
- The value of nodes is between 1 and 100.

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
    int sumEvenGrandparent(TreeNode* root) {
        
    }
};
```

## 1485. Clone Binary Tree With Random Pointer

A binary tree is given such that each node contains an additional random pointer which could point to any node in the tree or null.

Return a deep copy of the tree.

The tree is represented in the same input/output way as normal binary trees where each node is represented as a pair of [val, random_index] where:

- val: an integer representing Node.val
- random_index: the index of the node (in the input) where the random pointer points to, or null if it does not point to any node.

You will be given the tree in class Node and you should return the cloned tree in class NodeCopy. NodeCopy class is just a clone of Node class with the same attributes and constructors.

Example 1:

![](https://assets.leetcode.com/uploads/2020/06/17/clone_1.png)

```
Input: root = [[1,null],null,[4,3],[7,0]]
Output: [[1,null],null,[4,3],[7,0]]
Explanation: The original binary tree is [1,null,4,7].
The random pointer of node one is null, so it is represented as [1, null].
The random pointer of node 4 is node 7, so it is represented as [4, 3] 
where 3 is the index of node 7 in the array representing the tree.

The random pointer of node 7 is node 1, so it is represented as [7, 0] 
where 0 is the index of node 1 in the array representing the tree.
```

Example 2:

![](https://assets.leetcode.com/uploads/2020/06/17/clone_2.png)

```
Input: root = [[1,4],null,[1,0],null,[1,5],[1,5]]
Output: [[1,4],null,[1,0],null,[1,5],[1,5]]
Explanation: The random pointer of a node can be the node itself.
```

Example 3:

![](https://assets.leetcode.com/uploads/2020/06/17/clone_3.png)

```
Input: root = [[1,6],[2,5],[3,4],[4,3],[5,2],[6,1],[7,0]]
Output: [[1,6],[2,5],[3,4],[4,3],[5,2],[6,1],[7,0]]
```

Example 4:
```
Input: root = []
Output: []
```

Example 5:
```
Input: root = [[1,null],null,[2,null],null,[1,null]]
Output: [[1,null],null,[2,null],null,[1,null]]
```

Constraints:

- The number of nodes in the tree is in the range [0, 1000].
- Each node's value is between [1, 10^6].

Solution:
```cpp
/**
 * Definition for a Node.
 * struct Node {
 *     int val;
 *     Node *left;
 *     Node *right;
 *     Node *random;
 *     Node() : val(0), left(nullptr), right(nullptr), random(nullptr) {}
 *     Node(int x) : val(x), left(nullptr), right(nullptr), random(nullptr) {}
 *     Node(int x, Node *left, Node *right, Node *random) : val(x), left(left), right(right), random(random) {}
 * };
 */

class Solution {
public:
    NodeCopy* copyRandomBinaryTree(Node* root) {
        
    }
};
```

## 654. Maximum Binary Tree
Given an integer array with no duplicates. A maximum tree building on this array is defined as follow:

- The root is the maximum number in the array.
- The left subtree is the maximum tree constructed from left part subarray divided by the maximum number.
- The right subtree is the maximum tree constructed from right part subarray divided by the maximum number.

Construct the maximum tree by the given array and output the root node of this tree.

Example 1:
```
Input: [3,2,1,6,0,5]
Output: return the tree root node representing the following tree:

      6
    /   \
   3     5
    \    / 
     2  0   
       \
        1
```
Note:
- The size of the given array will be in the range [1,1000].

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
    TreeNode* constructMaximumBinaryTree(vector<int>& nums) {
        
    }
};
```

## 1008. Construct Binary Search Tree from Preorder Traversal
Return the root node of a binary search tree that matches the given preorder traversal.

(Recall that a binary search tree is a binary tree where for every node, any descendant of node.left has a value < node.val, and any descendant of node.right has a value > node.val.  Also recall that a preorder traversal displays the value of the node first, then traverses node.left, then traverses node.right.)

It's guaranteed that for the given test cases there is always possible to find a binary search tree with the given requirements.

Example 1:
```
Input: [8,5,1,7,10,12]
Output: [8,5,10,1,7,null,12]
```

![](https://assets.leetcode.com/uploads/2019/03/06/1266.png)

Constraints:
- 1 <= preorder.length <= 100
- 1 <= preorder[i] <= 10^8
- The values of preorder are distinct.

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
    TreeNode* bstFromPreorder(vector<int>& preorder) {
        
    }
};
```

## 701. Insert into a Binary Search Tree

Given the root node of a binary search tree (BST) and a value to be inserted into the tree, insert the value into the BST. Return the root node of the BST after the insertion. It is guaranteed that the new value does not exist in the original BST.

Note that there may exist multiple valid ways for the insertion, as long as the tree remains a BST after insertion. You can return any of them.

For example, 
```
Given the tree:
        4
       / \
      2   7
     / \
    1   3
And the value to insert: 5
```

You can return this binary search tree:
```
         4
       /   \
      2     7
     / \   /
    1   3 5
```

This tree is also valid:

```
         5
       /   \
      2     7
     / \   
    1   3
         \
          4
 ```

Constraints:

- The number of nodes in the given tree will be between 0 and 10^4.
- Each node will have a unique integer value from 0 to -10^8, inclusive.
- -10^8 <= val <= 10^8
- It's guaranteed that val does not exist in the original BST.

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
    TreeNode* insertIntoBST(TreeNode* root, int val) {
        
    }
};
```
