
# Tree

## 1469. Find All The Lonely Nodes
In a binary tree, a **lonely** node is a node that is the only child of its parent node. The root of the tree is not lonely because it does not have a parent node.

Given the root of a binary tree, return an array containing the values of all lonely nodes in the tree. Return the list **in any order**.

**Example 1:**

![](https://assets.leetcode.com/uploads/2020/06/03/e1.png)

```
Input: root = [1,2,3,null,4]
Output: [4]
Explanation: Light blue node is the only lonely node.
Node 1 is the root and is not lonely.
Nodes 2 and 3 have the same parent and are not lonely.
```

**Example 2:**

![](https://assets.leetcode.com/uploads/2020/06/03/e2.png)

```
Input: root = [7,1,4,6,null,5,3,null,null,null,null,null,2]
Output: [6,2]
Explanation: Light blue nodes are lonely nodes.
Please remember that order doesn't matter, [2,6] is also an acceptable answer.
```

**Example 3:**

![](https://assets.leetcode.com/uploads/2020/06/03/tree.png)

```
Input: root = [11,99,88,77,null,null,66,55,null,null,44,33,null,null,22]
Output: [77,55,33,66,44,22]
Explanation: Nodes 99 and 88 share the same parent. Node 11 is the root.
All other nodes are lonely.
```

**Example 4:**
```
Input: root = [197]
Output: []
```

**Example 5:**
```
Input: root = [31,null,78,null,28]
Output: [78,28]
```

**Constraints:**
- The number of nodes in the ```tree``` is in the range ```[1, 1000]```.
- Each node's value is between ```[1, 10^6]```.

**Solution:**

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
    vector<int> getLonelyNodes(TreeNode* root) {
        
    }
};
```

## 938. Range Sum of BST
Given the ```root``` node of a binary search tree, return the sum of values of all nodes with value between ```L``` and ```R ``` (inclusive).

The binary search tree is guaranteed to have unique values.

**Example 1:**

```
Input: root = [10,5,15,3,7,null,18], L = 7, R = 15
Output: 32
```

**Example 2:**
```
Input: root = [10,5,15,3,7,13,18,1,null,6], L = 6, R = 10
Output: 23
```

**Note:**
- The number of nodes in the tree is at most ```10000```.
- The final answer is guaranteed to be less than ```2^31```.

**Solution:**

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
    int rangeSumBST(TreeNode* root, int L, int R) {
        
    }
};
```
