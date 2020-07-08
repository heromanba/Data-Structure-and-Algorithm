
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

## 1305. All Elements in Two Binary Search Trees

Given two binary search trees root1 and root2.

Return a list containing all the integers from both trees sorted in ascending order.

Example 1:

![](https://assets.leetcode.com/uploads/2019/12/18/q2-e1.png)

```
Input: root1 = [2,1,4], root2 = [1,0,3]
Output: [0,1,1,2,3,4]
```

Example 2:

```
Input: root1 = [0,-10,10], root2 = [5,1,7,0,2]
Output: [-10,0,0,1,2,5,7,10]
```

Example 3:

```
Input: root1 = [], root2 = [5,1,7,0,2]
Output: [0,1,2,5,7]
```

Example 4:

```
Input: root1 = [0,-10,10], root2 = []
Output: [-10,0,10]
```

Example 5:

![](https://assets.leetcode.com/uploads/2019/12/18/q2-e5-.png)

```
Input: root1 = [1,null,8], root2 = [8,1]
Output: [1,1,8,8]
```

Constraints:

- Each tree has at most 5000 nodes.
- Each node's value is between [-10^5, 10^5].

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
    vector<int> getAllElements(TreeNode* root1, TreeNode* root2) {
        
    }
};
```

## 894. All Possible Full Binary Trees

A full binary tree is a binary tree where each node has exactly 0 or 2 children.

Return a list of all possible full binary trees with N nodes.  Each element of the answer is the root node of one possible tree.

Each node of each tree in the answer must have node.val = 0.

You may return the final list of trees in any order.

Example 1:

```
Input: 7
Output: 
[
    [0,0,0,null,null,0,0,null,null,0,0],
    [0,0,0,null,null,0,0,0,0],
    [0,0,0,0,0,0,0],
    [0,0,0,0,0,null,null,null,null,0,0],
    [0,0,0,0,0,null,null,0,0]
]

Explanation:
```

![](https://s3-lc-upload.s3.amazonaws.com/uploads/2018/08/22/fivetrees.png)

Note:

- 1 <= N <= 20

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
    vector<TreeNode*> allPossibleFBT(int N) {
        
    }
};
```

## 814. Binary Tree Pruning

We are given the head node root of a binary tree, where additionally every node's value is either a 0 or a 1.

Return the same tree where every subtree (of the given tree) not containing a 1 has been removed.

(Recall that the subtree of a node X is X, plus every node that is a descendant of X.)

```
Example 1:
Input: [1,null,0,0,1]
Output: [1,null,0,null,1]
 
Explanation: 
Only the red nodes satisfy the property "every subtree not containing a 1".
The diagram on the right represents the answer.
```

![](https://s3-lc-upload.s3.amazonaws.com/uploads/2018/04/06/1028_2.png)

```
Example 2:
Input: [1,0,1,0,0,0,1]
Output: [1,null,1,null,1]
```

![](https://s3-lc-upload.s3.amazonaws.com/uploads/2018/04/06/1028_1.png)

```
Example 3:
Input: [1,1,0,1,1,0,1,0]
Output: [1,1,0,1,1,null,1]
```

![](https://s3-lc-upload.s3.amazonaws.com/uploads/2018/04/05/1028.png)

Note:

- The binary tree will have at most 100 nodes.
- The value of each node will only be 0 or 1.

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
    TreeNode* pruneTree(TreeNode* root) {
        
    }
};
```

## 1261. Find Elements in a Contaminated Binary Tree

Given a binary tree with the following rules:

- root.val == 0
- If treeNode.val == x and treeNode.left != null, then treeNode.left.val == 2 * x + 1
- If treeNode.val == x and treeNode.right != null, then treeNode.right.val == 2 * x + 2
Now the binary tree is contaminated, which means all treeNode.val have been changed to -1.

You need to first recover the binary tree and then implement the FindElements class:

- FindElements(TreeNode* root) Initializes the object with a contamined binary tree, you need to recover it first.
- bool find(int target) Return if the target value exists in the recovered binary tree.

Example 1:

![](https://assets.leetcode.com/uploads/2019/11/06/untitled-diagram-4-1.jpg)

```
Input
["FindElements","find","find"]
[[[-1,null,-1]],[1],[2]]
Output
[null,false,true]
Explanation
FindElements findElements = new FindElements([-1,null,-1]); 
findElements.find(1); // return False 
findElements.find(2); // return True 
```

Example 2:

![](https://assets.leetcode.com/uploads/2019/11/06/untitled-diagram-4.jpg)

```
Input
["FindElements","find","find","find"]
[[[-1,-1,-1,-1,-1]],[1],[3],[5]]
Output
[null,true,true,false]
Explanation
FindElements findElements = new FindElements([-1,-1,-1,-1,-1]);
findElements.find(1); // return True
findElements.find(3); // return True
findElements.find(5); // return False
```

Example 3:

![](https://assets.leetcode.com/uploads/2019/11/07/untitled-diagram-4-1-1.jpg)

```
Input
["FindElements","find","find","find","find"]
[[[-1,null,-1,-1,null,-1]],[2],[3],[4],[5]]
Output
[null,true,false,false,true]
Explanation
FindElements findElements = new FindElements([-1,null,-1,-1,null,-1]);
findElements.find(2); // return True
findElements.find(3); // return False
findElements.find(4); // return False
findElements.find(5); // return True
```

Constraints:

- TreeNode.val == -1
- The height of the binary tree is less than or equal to 20
- The total number of nodes is between [1, 10^4]
- Total calls of find() is between [1, 10^4]
- 0 <= target <= 10^6

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
class FindElements {
public:
    FindElements(TreeNode* root) {
        
    }
    
    bool find(int target) {
        
    }
};

/**
 * Your FindElements object will be instantiated and called as such:
 * FindElements* obj = new FindElements(root);
 * bool param_1 = obj->find(target);
 */
```

## 1325. Delete Leaves With a Given Value

Given a binary tree root and an integer target, delete all the leaf nodes with value target.

Note that once you delete a leaf node with value target, if it's parent node becomes a leaf node and has the value target, it should also be deleted (you need to continue doing that until you can't).

Example 1:

![](https://assets.leetcode.com/uploads/2020/01/09/sample_1_1684.png)

```
Input: root = [1,2,3,2,null,2,4], target = 2
Output: [1,null,3,null,4]
Explanation: Leaf nodes in green with value (target = 2) are removed (Picture in left). 
After removing, new nodes become leaf nodes with value (target = 2) (Picture in center).
```

Example 2:

![](https://assets.leetcode.com/uploads/2020/01/09/sample_2_1684.png)

```
Input: root = [1,3,3,3,2], target = 3
Output: [1,3,null,null,2]
```

Example 3:

![](https://assets.leetcode.com/uploads/2020/01/15/sample_3_1684.png)

```
Input: root = [1,2,null,2,null,2], target = 2
Output: [1]
Explanation: Leaf nodes in green with value (target = 2) are removed at each step.
```

Example 4:
```
Input: root = [1,1,1], target = 1
Output: []
```

Example 5:
```
Input: root = [1,2,3], target = 1
Output: [1,2,3]
```

Constraints:

- 1 <= target <= 1000
- The given binary tree will have between 1 and 3000 nodes.
- Each node's value is between [1, 1000].

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
    TreeNode* removeLeafNodes(TreeNode* root, int target) {
        
    }
};
```

## 1104. Path In Zigzag Labelled Binary Tree
In an infinite binary tree where every node has two children, the nodes are labelled in row order.

In the odd numbered rows (ie., the first, third, fifth,...), the labelling is left to right, while in the even numbered rows (second, fourth, sixth,...), the labelling is right to left.

![](https://assets.leetcode.com/uploads/2019/06/24/tree.png)

Given the label of a node in this tree, return the labels in the path from the root of the tree to the node with that label.

Example 1:
```
Input: label = 14
Output: [1,3,4,14]
```

Example 2:
```
Input: label = 26
Output: [1,2,6,10,26]
```

Constraints:

- 1 <= label <= 10^6

Solution:

```cpp
class Solution {
public:
    vector<int> pathInZigZagTree(int label) {
        
    }
};
```

## 366. Find Leaves of Binary Tree

Given a binary tree, collect a tree's nodes as if you were doing this: Collect and remove all leaves, repeat until the tree is empty.

Example:

```
Input: [1,2,3,4,5]
  
          1
         / \
        2   3
       / \     
      4   5    

Output: [[4,5,3],[2],[1]]
```

Explanation:

1. Removing the leaves [4,5,3] would result in this tree:
```
          1
         / 
        2          
 ```

2. Now removing the leaf [2] would result in this tree:
```
          1          
 ```

3. Now removing the leaf [1] would result in the empty tree:
```
          []  
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
    vector<vector<int>> findLeaves(TreeNode* root) {
        
    }
};
```

## 1448. Count Good Nodes in Binary Tree

Given a binary tree root, a node X in the tree is named good if in the path from root to X there are no nodes with a value greater than X.

Return the number of good nodes in the binary tree.

Example 1:

![](https://assets.leetcode.com/uploads/2020/04/02/test_sample_1.png)

```
Input: root = [3,1,4,3,null,1,5]
Output: 4
Explanation: Nodes in blue are good.
Root Node (3) is always a good node.
Node 4 -> (3,4) is the maximum value in the path starting from the root.
Node 5 -> (3,4,5) is the maximum value in the path
Node 3 -> (3,1,3) is the maximum value in the path.
```

Example 2:

![](https://assets.leetcode.com/uploads/2020/04/02/test_sample_2.png)

```
Input: root = [3,3,null,4,2]
Output: 3
Explanation: Node 2 -> (3, 3, 2) is not good, because "3" is higher than it.
```

Example 3:
```
Input: root = [1]
Output: 1
Explanation: Root is considered as good.
```

Constraints:

- The number of nodes in the binary tree is in the range [1, 10^5].
- Each node's value is between [-10^4, 10^4].

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
    int goodNodes(TreeNode* root) {
        
    }
};
```

## 979. Distribute Coins in Binary Tree

Given the root of a binary tree with N nodes, each node in the tree has node.val coins, and there are N coins total.

In one move, we may choose two adjacent nodes and move one coin from one node to another.  (The move may be from parent to child, or from child to parent.)

Return the number of moves required to make every node have exactly one coin.

Example 1:

![](https://assets.leetcode.com/uploads/2019/01/18/tree1.png)

```
Input: [3,0,0]
Output: 2
Explanation: From the root of the tree, we move one coin to its left child, 
and one coin to its right child.
```

Example 2:

![](https://assets.leetcode.com/uploads/2019/01/18/tree2.png)

```cpp
Input: [0,3,0]
Output: 3
Explanation: From the left child of the root, we move two coins to the 
root [taking two moves].  Then, we move one coin from the root of the 
tree to the right child.
```

Example 3:

![](https://assets.leetcode.com/uploads/2019/01/18/tree3.png)

```
Input: [1,0,2]
Output: 2
```

Example 4:

![](https://assets.leetcode.com/uploads/2019/01/18/tree4.png)

```
Input: [1,0,0,null,3]
Output: 4
```

Note:

- 1<= N <= 100
- 0 <= node.val <= N

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
    int distributeCoins(TreeNode* root) {
        
    }
};
```

## 1457. Pseudo-Palindromic Paths in a Binary Tree

Given a binary tree where node values are digits from 1 to 9. A path in the binary tree is said to be pseudo-palindromic if at least one permutation of the node values in the path is a palindrome.

Return the number of pseudo-palindromic paths going from the root node to leaf nodes.

Example 1:

![](https://assets.leetcode.com/uploads/2020/05/06/palindromic_paths_1.png)

```
Input: root = [2,3,1,3,1,null,1]
Output: 2 
Explanation: The figure above represents the given binary tree. There are three 
paths going from the root node to leaf nodes: the red path [2,3,3], the green 
path [2,1,1], and the path [2,3,1]. Among these paths only red path and green 
path are pseudo-palindromic paths since the red path [2,3,3] can be rearranged 
in [3,2,3] (palindrome) and the green path [2,1,1] can be rearranged in [1,2,1] 
(palindrome).
```

Example 2:

![](https://assets.leetcode.com/uploads/2020/05/07/palindromic_paths_2.png)

```
Input: root = [2,1,1,1,3,null,null,null,null,null,1]
Output: 1 
Explanation: The figure above represents the given binary tree. There are 
three paths going from the root node to leaf nodes: the green path [2,1,1], 
the path [2,1,3,1], and the path [2,1]. Among these paths only the green path 
is pseudo-palindromic since [2,1,1] can be rearranged in [1,2,1] (palindrome).
```
Example 3:
```
Input: root = [9]
Output: 1
```

Constraints:

- The given binary tree will have between 1 and 10^5 nodes.
- Node values are digits from 1 to 9.

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
    int pseudoPalindromicPaths (TreeNode* root) {
        
    }
};
```

## 1123. Lowest Common Ancestor of Deepest Leaves
Given a rooted binary tree, return the lowest common ancestor of its deepest leaves.

Recall that:

- The node of a binary tree is a leaf if and only if it has no children
- The depth of the root of the tree is 0, and if the depth of a node is d, the depth of each of its children is d+1.
- The lowest common ancestor of a set S of nodes is the node A with the largest depth such that every node in S is in the subtree with root A.
 

Example 1:
```
Input: root = [1,2,3]
Output: [1,2,3]
Explanation: 
The deepest leaves are the nodes with values 2 and 3.
The lowest common ancestor of these leaves is the node with value 1.
The answer returned is a TreeNode object (not an array) with serialization "[1,2,3]".
```

Example 2:
```
Input: root = [1,2,3,4]
Output: [4]
```

Example 3:
```
Input: root = [1,2,3,4,5]
Output: [2,4,5]
``` 

Constraints:

- The given tree will have between 1 and 1000 nodes.
- Each node of the tree will have a distinct value between 1 and 1000.

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
    TreeNode* lcaDeepestLeaves(TreeNode* root) {
        
    }
};
```

## 1110. Delete Nodes And Return Forest

Given the root of a binary tree, each node in the tree has a distinct value.

After deleting all nodes with a value in to_delete, we are left with a forest (a disjoint union of trees).

Return the roots of the trees in the remaining forest.  You may return the result in any order.

Example 1:

![](https://assets.leetcode.com/uploads/2019/07/01/screen-shot-2019-07-01-at-53836-pm.png)
```
Input: root = [1,2,3,4,5,6,7], to_delete = [3,5]
Output: [[1,2,null,4],[6],[7]]
```

Constraints:

- The number of nodes in the given tree is at most 1000.
- Each node has a distinct value between 1 and 1000.
- to_delete.length <= 1000
- to_delete contains distinct values between 1 and 1000.

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
    vector<TreeNode*> delNodes(TreeNode* root, vector<int>& to_delete) {
        
    }
};
```

## 889. Construct Binary Tree from Preorder and Postorder Traversal
Return any binary tree that matches the given preorder and postorder traversals.

Values in the traversals pre and post are distinct positive integers.

 

Example 1:
```
Input: pre = [1,2,4,5,3,6,7], post = [4,5,2,6,7,3,1]
Output: [1,2,3,4,5,6,7]
```

Note:

- 1 <= pre.length == post.length <= 30
- pre[] and post[] are both permutations of 1, 2, ..., pre.length.
- It is guaranteed an answer exists. If there exists multiple answers, you can return any of them.

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
    TreeNode* constructFromPrePost(vector<int>& pre, vector<int>& post) {
        
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

## 951. Flip Equivalent Binary Trees

For a binary tree T, we can define a flip operation as follows: choose any node, and swap the left and right child subtrees.

A binary tree X is flip equivalent to a binary tree Y if and only if we can make X equal to Y after some number of flip operations.

Write a function that determines whether two binary trees are flip equivalent.  The trees are given by root nodes root1 and root2.

Example 1:
```
Input: root1 = [1,2,3,4,5,6,null,null,null,7,8], 
root2 = [1,3,2,null,6,4,5,null,null,null,null,8,7]

Output: true

Explanation: We flipped at nodes with values 1, 3, and 5.
```

![](https://assets.leetcode.com/uploads/2018/11/29/tree_ex.png)

Note:

- Each tree will have at most 100 nodes.
- Each value in each tree will be a unique integer in the range [0, 99].

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
    bool flipEquiv(TreeNode* root1, TreeNode* root2) {
        
    }
};
```

## 1026. Maximum Difference Between Node and Ancestor

Given the root of a binary tree, find the maximum value V for which there exists different nodes A and B where V = |A.val - B.val| and A is an ancestor of B.

(A node A is an ancestor of B if either: any child of A is equal to B, or any child of A is an ancestor of B.)

Example 1:

![](https://assets.leetcode.com/uploads/2019/09/09/2whqcep.jpg)

```
Input: [8,3,10,1,6,null,14,null,null,4,7,13]
Output: 7
Explanation: 
We have various ancestor-node differences, 
some of which are given below :

|8 - 3| = 5
|3 - 7| = 4
|8 - 1| = 7
|10 - 13| = 3

Among all possible differences, 
the maximum value of 7 is obtained by |8 - 1| = 7.
```

Note:

- The number of nodes in the tree is between 2 and 5000.
- Each node will have value between 0 and 100000.

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
    int maxAncestorDiff(TreeNode* root) {
        
    }
};
```

## 429. N-ary Tree Level Order Traversal

Given an n-ary tree, return the level order traversal of its nodes' values.

Nary-Tree input serialization is represented in their level order traversal, each group of children is separated by the null value (See examples).

Example 1:

![](https://assets.leetcode.com/uploads/2018/10/12/narytreeexample.png)

```
Input: root = [1,null,3,2,4,null,5,6]
Output: [[1],[3,2,4],[5,6]]
```

Example 2:

![](https://assets.leetcode.com/uploads/2019/11/08/sample_4_964.png)

```
Input: root = 
[1,null,2,3,4,5,null,null,6,7,null,8,null,9,10,
 null,null,11,null,12,null,13,null,null,14]
 
Output: [[1],[2,3,4,5],[6,7,8,9,10],[11,12,13],[14]]
```

Constraints:

- The height of the n-ary tree is less than or equal to 1000
- The total number of nodes is between [0, 10^4]

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
    vector<vector<int>> levelOrder(Node* root) {
        
    }
};
```

## 1466. Reorder Routes to Make All Paths Lead to the City Zero

There are n cities numbered from 0 to n-1 and n-1 roads such that there is only one way to travel between two different cities (this network form a tree). Last year, The ministry of transport decided to orient the roads in one direction because they are too narrow.

Roads are represented by connections where connections[i] = [a, b] represents a road from city a to b.

This year, there will be a big event in the capital (city 0), and many people want to travel to this city.

Your task consists of reorienting some roads such that each city can visit the city 0. Return the minimum number of edges changed.

It's guaranteed that each city can reach the city 0 after reorder.

Example 1:

![](https://assets.leetcode.com/uploads/2020/05/13/sample_1_1819.png)

```
Input: n = 6, connections = [[0,1],[1,3],[2,3],[4,0],[4,5]]
Output: 3

Explanation: Change the direction of edges show in red such 
that each node can reach the node 0 (capital).
```

Example 2:

![](https://assets.leetcode.com/uploads/2020/05/13/sample_2_1819.png)

```
Input: n = 5, connections = [[1,0],[1,2],[3,2],[3,4]]
Output: 2
Explanation: Change the direction of edges show in red such that 
each node can reach the node 0 (capital).
```

Example 3:

```
Input: n = 3, connections = [[1,0],[2,0]]
Output: 0
```

Constraints:

- 2 <= n <= 5 * 10^4
- connections.length == n-1
- connections[i].length == 2
- 0 <= connections[i][0], connections[i][1] <= n-1
- connections[i][0] != connections[i][1]

Solution:
```cpp
class Solution {
public:
    int minReorder(int n, vector<vector<int>>& connections) {
        
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
        vector<int> vec_root;
        if (root == NULL)
            return vec_root;
        
        vector<int> vec_left;
        vector<int> vec_right;
        
        if (root->left != NULL)
            vec_left = inorderTraversal(root->left);
        vec_root.insert(vec_root.end(), vec_left.begin(), vec_left.end());
        
        vec_root.push_back(root->val);
        
        if (root->right != NULL)
            vec_right = inorderTraversal(root->right);
        vec_root.insert(vec_root.end(), vec_right.begin(), vec_right.end());
        
        return vec_root;
    }
};
```

## 998. Maximum Binary Tree II

We are given the root node of a maximum tree: a tree where every node has a value greater than any other value in its subtree.

Just as in the previous problem, the given tree was constructed from an list A (root = Construct(A)) recursively with the following Construct(A) routine:

- If A is empty, return null.
- Otherwise, let A[i] be the largest element of A.  Create a root node with value A[i].
- The left child of root will be Construct([A[0], A[1], ..., A[i-1]])
- The right child of root will be Construct([A[i+1], A[i+2], ..., A[A.length - 1]])
- Return root.

Note that we were not given A directly, only a root node root = Construct(A).

Suppose B is a copy of A with the value val appended to it.  It is guaranteed that B has unique values.

Return Construct(B).

Example 1:

![](https://assets.leetcode.com/uploads/2019/02/21/maximum-binary-tree-1-2.png)

```
Input: root = [4,1,3,null,null,2], val = 5
Output: [5,4,null,1,3,null,null,2]
Explanation: A = [1,4,2,3], B = [1,4,2,3,5]
```

Example 2:

![](https://assets.leetcode.com/uploads/2019/02/21/maximum-binary-tree-2-2.png)

```
Input: root = [5,2,4,null,1], val = 3
Output: [5,2,4,null,1,null,3]
Explanation: A = [2,1,5,4], B = [2,1,5,4,3]
```

Example 3:

![](https://assets.leetcode.com/uploads/2019/02/21/maximum-binary-tree-3-2.png)

```
Input: root = [5,2,3,null,1], val = 4
Output: [5,2,4,null,1,3]
Explanation: A = [2,1,5,3], B = [2,1,5,3,4]
```

Constraints:

- 1 <= B.length <= 100

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
    TreeNode* insertIntoMaxTree(TreeNode* root, int val) {
        
    }
};
```

## 1120. Maximum Average Subtree

Given the root of a binary tree, find the maximum average value of any subtree of that tree.

(A subtree of a tree is any node of that tree plus all its descendants. The average value of a tree is the sum of its values, divided by the number of nodes.) 

Example 1:

![](https://assets.leetcode.com/uploads/2019/04/09/1308_example_1.png)

```
Input: [5,6,1]
Output: 6.00000
Explanation: 
For the node with value = 5 we have an average of (5 + 6 + 1) / 3 = 4.
For the node with value = 6 we have an average of 6 / 1 = 6.
For the node with value = 1 we have an average of 1 / 1 = 1.
So the answer is 6 which is the maximum.
```

Note:

- The number of nodes in the tree is between 1 and 5000.
- Each node will have a value between 0 and 100000.
- Answers will be accepted as correct if they are within 10^-5 of the correct answer.

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
    double maximumAverageSubtree(TreeNode* root) {
        
    }
};
```

## 513. Find Bottom Left Tree Value

Given a binary tree, find the leftmost value in the last row of the tree.

Example 1:
```
Input:

    2
   / \
  1   3

Output:
1
```

Example 2:
```
Input:

        1
       / \
      2   3
     /   / \
    4   5   6
       /
      7

Output:
7
```
Note: You may assume the tree (i.e., the given root node) is not NULL.

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
    int findBottomLeftValue(TreeNode* root) {
        
    }
};
```

515. Find Largest Value in Each Tree Row

You need to find the largest value in each row of a binary tree.

Example:
```
Input: 

          1
         / \
        3   2
       / \   \  
      5   3   9 

Output: [1, 3, 9]
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
    vector<int> largestValues(TreeNode* root) {
        
    }
};
```
