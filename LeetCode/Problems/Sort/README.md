
# Sort

Sorted by frequency, only includes green and yellow.

## 148. Sort List

Sort a linked list in O(n log n) time using constant space complexity.

Example 1:
```
Input: 4->2->1->3
Output: 1->2->3->4
```
Example 2:
```
Input: -1->5->3->4->0
Output: -1->0->3->4->5
```

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
    ListNode* sortList(ListNode* head) {
        
    }
};
```

## 56. Merge Intervals

Given a collection of intervals, merge all overlapping intervals.

Example 1:
```
Input: [[1,3],[2,6],[8,10],[15,18]]
Output: [[1,6],[8,10],[15,18]]
Explanation: Since intervals [1,3] and [2,6] overlaps, merge them into [1,6].
```
Example 2:
```
Input: [[1,4],[4,5]]
Output: [[1,5]]
Explanation: Intervals [1,4] and [4,5] are considered overlapping.
```
NOTE: input types have been changed on April 15, 2019. Please reset to 
default code definition to get new method signature.

Solution:
```cpp
class Solution {
public:
    vector<vector<int>> merge(vector<vector<int>>& intervals) {
        
    }
};
```

## 315. Count of Smaller Numbers After Self

You are given an integer array nums and you have to return a new counts array.
The counts array has the property where counts[i] is the number of smaller elements to the right of nums[i].

Example:
```
Input: [5,2,6,1]
Output: [2,1,1,0] 
Explanation:
To the right of 5 there are 2 smaller elements (2 and 1).
To the right of 2 there is only 1 smaller element (1).
To the right of 6 there is 1 smaller element (1).
To the right of 1 there is 0 smaller element.
```

Solution:
```cpp
class Solution {
public:
    vector<int> countSmaller(vector<int>& nums) {
        
    }
};
```

## 147. Insertion Sort List

Sort a linked list using insertion sort.


A graphical example of insertion sort. The partial sorted list (black) initially contains only the first element in the list.
With each iteration one element (red) is removed from the input data and inserted in-place into the sorted list
 

Algorithm of Insertion Sort:

- Insertion sort iterates, consuming one input element each repetition, and growing a sorted output list.
- At each iteration, insertion sort removes one element from the input data, finds the location it belongs within the sorted list, and inserts it there.
- It repeats until no input elements remain.

Example 1:
```
Input: 4->2->1->3
Output: 1->2->3->4
```
Example 2:
```
Input: -1->5->3->4->0
Output: -1->0->3->4->5
```

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
    ListNode* insertionSortList(ListNode* head) {
        
    }
};
```

## 179. Largest Number

Given a list of non negative integers, arrange them such that they form the largest number.

Example 1:
```
Input: [10,2]
Output: "210"
```
Example 2:
```
Input: [3,30,34,5,9]
Output: "9534330"
```
Note: The result may be very large, so you need to return a string instead of an integer.

Solution:
```cpp
class Solution {
public:
    string largestNumber(vector<int>& nums) {
        
    }
};
```

## 349. Intersection of Two Arrays

Given two arrays, write a function to compute their intersection.

Example 1:
```
Input: nums1 = [1,2,2,1], nums2 = [2,2]
Output: [2]
```
Example 2:
```
Input: nums1 = [4,9,5], nums2 = [9,4,9,8,4]
Output: [9,4]
```
Note:

- Each element in the result must be unique.
- The result can be in any order.

Solution:
```cpp
class Solution {
public:
    vector<int> intersection(vector<int>& nums1, vector<int>& nums2) {
        
    }
};
```

## 253. Meeting Rooms II

Given an array of meeting time intervals consisting of start and end times [[s1,e1],[s2,e2],...] (si < ei), find the minimum number of conference rooms required.

Example 1:
```
Input: [[0, 30],[5, 10],[15, 20]]
Output: 2
```
Example 2:
```
Input: [[7,10],[2,4]]
Output: 1
```
NOTE: input types have been changed on April 15, 2019. Please reset to default code definition to get new method signature.

Solution:
```cpp
class Solution {
public:
    int minMeetingRooms(vector<vector<int>>& intervals) {
        
    }
};
```

## 164. Maximum Gap

Given an unsorted array, find the maximum difference between the successive elements in its sorted form.

Return 0 if the array contains less than 2 elements.

Example 1:
```
Input: [3,6,9,1]
Output: 3
Explanation: The sorted form of the array is [1,3,6,9], either
             (3,6) or (6,9) has the maximum difference 3.
```
Example 2:
```
Input: [10]
Output: 0
Explanation: The array contains less than 2 elements, therefore return 0.
```
Note:

- You may assume all elements in the array are non-negative integers and fit in the 32-bit signed integer range.
- Try to solve it in linear time/space.

Solution:
```cpp
class Solution {
public:
    int maximumGap(vector<int>& nums) {
        
    }
};
```

## 242. Valid Anagram

Given two strings s and t , write a function to determine if t is an anagram of s.

Example 1:
```
Input: s = "anagram", t = "nagaram"
Output: true
```
Example 2:
```
Input: s = "rat", t = "car"
Output: false
```
Note:
You may assume the string contains only lowercase alphabets.

Follow up:
What if the inputs contain unicode characters? How would you adapt your solution to such case?

Solution:
```cpp
class Solution {
public:
    bool isAnagram(string s, string t) {
        
    }
};
```

## 220. Contains Duplicate III

Given an array of integers, find out whether there are two distinct indices i and j in the array such that the absolute difference between nums[i] and nums[j] is at most t and the absolute difference between i and j is at most k.

Example 1:
```
Input: nums = [1,2,3,1], k = 3, t = 0
Output: true
```
Example 2:
```
Input: nums = [1,0,1,1], k = 1, t = 2
Output: true
```
Example 3:
```
Input: nums = [1,5,9,1,5,9], k = 2, t = 3
Output: false
```

Solution:
```cpp
class Solution {
public:
    bool containsNearbyAlmostDuplicate(vector<int>& nums, int k, int t) {
        
    }
};
```

## 327. Count of Range Sum

Given an integer array nums, return the number of range sums that lie in [lower, upper] inclusive.
Range sum S(i, j) is defined as the sum of the elements in nums between indices i and j (i ≤ j), inclusive.

Note:
A naive algorithm of O(n2) is trivial. You MUST do better than that.

Example:
```
Input: nums = [-2,5,-1], lower = -2, upper = 2,
Output: 3 

Explanation: The three ranges are : [0,0], [2,2], [0,2] and 
their respective sums are: -2, -1, 2.
```

Solution:
```cpp
class Solution {
public:
    int countRangeSum(vector<int>& nums, int lower, int upper) {
        
    }
};
```

## 280. Wiggle Sort

Given an unsorted array nums, reorder it in-place such that nums[0] <= nums[1] >= nums[2] <= nums[3]....

Example:
```
Input: nums = [3,5,2,1,6,4]
Output: One possible answer is [3,5,1,6,2,4]
```

Solution:
```cpp
class Solution {
public:
    void wiggleSort(vector<int>& nums) {
        
    }
};
```

## 75. Sort Colors

Given an array with n objects colored red, white or blue, sort them in-place so that objects of the same color are adjacent, with the colors in the order red, white and blue.

Here, we will use the integers 0, 1, and 2 to represent the color red, white, and blue respectively.

Note: You are not suppose to use the library's sort function for this problem.

Example:
```
Input: [2,0,2,1,1,0]
Output: [0,0,1,1,2,2]
```
Follow up:

- A rather straight forward solution is a two-pass algorithm using counting sort.
First, iterate the array counting number of 0's, 1's, and 2's, then overwrite array with total number of 0's, then 1's and followed by 2's.
- Could you come up with a one-pass algorithm using only constant space?

Solution:
```cpp
class Solution {
public:
    void sortColors(vector<int>& nums) {
        
    }
};
```

## 973. K Closest Points to Origin

We have a list of points on the plane.  Find the K closest points to the origin (0, 0).

(Here, the distance between two points on a plane is the Euclidean distance.)

You may return the answer in any order.  The answer is guaranteed to be unique (except for the order that it is in.)

 

Example 1:
```
Input: points = [[1,3],[-2,2]], K = 1
Output: [[-2,2]]
Explanation: 
The distance between (1, 3) and the origin is sqrt(10).
The distance between (-2, 2) and the origin is sqrt(8).
Since sqrt(8) < sqrt(10), (-2, 2) is closer to the origin.
We only want the closest K = 1 points from the origin, so the answer is just [[-2,2]].
```
Example 2:
```
Input: points = [[3,3],[5,-1],[-2,4]], K = 2
Output: [[3,3],[-2,4]]
(The answer [[-2,4],[3,3]] would also be accepted.)
``` 

Note:

- 1 <= K <= points.length <= 10000
- -10000 < points[i][0] < 10000
- -10000 < points[i][1] < 10000

Solution:
```cpp
class Solution {
public:
    vector<vector<int>> kClosest(vector<vector<int>>& points, int K) {
        
    }
};
```

## 324. Wiggle Sort II

Given an unsorted array nums, reorder it such that nums[0] < nums[1] > nums[2] < nums[3]....

Example 1:
```
Input: nums = [1, 5, 1, 1, 6, 4]
Output: One possible answer is [1, 4, 1, 5, 1, 6].
```
Example 2:
```
Input: nums = [1, 3, 2, 2, 3, 1]
Output: One possible answer is [2, 3, 1, 3, 1, 2].
```
Note:
You may assume all input has valid answer.

Follow Up:
Can you do it in O(n) time and/or in-place with O(1) extra space?

Solution:
```cpp
class Solution {
public:
    void wiggleSort(vector<int>& nums) {
        
    }
};
```

## 969. Pancake Sorting

Given an array A, we can perform a pancake flip: We choose some positive integer k <= A.length, then reverse the order of the first k elements of A.  We want to perform zero or more pancake flips (doing them one after another in succession) to sort the array A.

Return the k-values corresponding to a sequence of pancake flips that sort A.  Any valid answer that sorts the array within 10 * A.length flips will be judged as correct.

 

Example 1:
```
Input: [3,2,4,1]
Output: [4,2,4,3]
Explanation: 
We perform 4 pancake flips, with k values 4, 2, 4, and 3.
Starting state: A = [3, 2, 4, 1]
After 1st flip (k=4): A = [1, 4, 2, 3]
After 2nd flip (k=2): A = [4, 1, 2, 3]
After 3rd flip (k=4): A = [3, 2, 1, 4]
After 4th flip (k=3): A = [1, 2, 3, 4], which is sorted. 
```
Example 2:
```
Input: [1,2,3]
Output: []
Explanation: The input is already sorted, so there is no need 
to flip anything. Note that other answers, such as [3, 3], 
would also be accepted.
```

Note:

- 1 <= A.length <= 100
- A[i] is a permutation of [1, 2, ..., A.length]

Solution:
```cpp
class Solution {
public:
    vector<int> pancakeSort(vector<int>& A) {
        
    }
};
```

## 1329. Sort the Matrix Diagonally

Given a m * n matrix mat of integers, sort it diagonally in ascending order from the top-left to the bottom-right then return the sorted array.

 ![](https://assets.leetcode.com/uploads/2020/01/21/1482_example_1_2.png)

Example 1:

```
Input: mat = [[3,3,1,1],[2,2,1,2],[1,1,1,2]]
Output: [[1,1,1,1],[1,2,2,2],[1,2,3,3]]
```

Constraints:

- m == mat.length
- n == mat[i].length
- 1 <= m, n <= 100
- 1 <= mat[i][j] <= 100

Solution:
```cpp
class Solution {
public:
    vector<vector<int>> diagonalSort(vector<vector<int>>& mat) {
        
    }
};
```

## 767. Reorganize String

Given a string S, check if the letters can be rearranged so that two characters that are adjacent to each other are not the same.

If possible, output any possible result.  If not possible, return the empty string.

Example 1:
```
Input: S = "aab"
Output: "aba"
```
Example 2:
```
Input: S = "aaab"
Output: ""
```
Note:

- S will consist of lowercase letters and have length in range [1, 500].

Solution:
```cpp
class Solution {
public:
    string reorganizeString(string S) {
        
    }
};
```

## 350. Intersection of Two Arrays II

Given two arrays, write a function to compute their intersection.

Example 1:
```
Input: nums1 = [1,2,2,1], nums2 = [2,2]
Output: [2,2]
```
Example 2:
```
Input: nums1 = [4,9,5], nums2 = [9,4,9,8,4]
Output: [4,9]
```
Note:

- Each element in the result should appear as many times as it shows in both arrays.
- The result can be in any order.

Follow up:

- What if the given array is already sorted? How would you optimize your algorithm?
- What if nums1's size is small compared to nums2's size? Which algorithm is better?
- What if elements of nums2 are stored on disk, and the memory is limited such that you cannot load all elements into the memory at once?

Solution:
```cpp
class Solution {
public:
    vector<int> intersect(vector<int>& nums1, vector<int>& nums2) {
        
    }
};
```

## 296. Best Meeting Point

A group of two or more people wants to meet and minimize the total travel distance. You are given a 2D grid of values 0 or 1, where each 1 marks the home of someone in the group. The distance is calculated using Manhattan Distance, where distance(p1, p2) = |p2.x - p1.x| + |p2.y - p1.y|.

Example:
```
Input: 

1 - 0 - 0 - 0 - 1
|   |   |   |   |
0 - 0 - 0 - 0 - 0
|   |   |   |   |
0 - 0 - 1 - 0 - 0

Output: 6 

Explanation: Given three people living at (0,0), (0,4), and (2,2):
             The point (0,2) is an ideal meeting point, as the total travel distance 
             of 2+2+2=6 is minimal. So return 6.
```

Solution:
```cpp
class Solution {
public:
    int minTotalDistance(vector<vector<int>>& grid) {
        
    }
};
```

## 57. Insert Interval

Given a set of non-overlapping intervals, insert a new interval into the intervals (merge if necessary).

You may assume that the intervals were initially sorted according to their start times.

Example 1:
```
Input: intervals = [[1,3],[6,9]], newInterval = [2,5]
Output: [[1,5],[6,9]]
```

Example 2:
```
Input: intervals = [[1,2],[3,5],[6,7],[8,10],[12,16]], newInterval = [4,8]
Output: [[1,2],[3,10],[12,16]]
Explanation: Because the new interval [4,8] overlaps with [3,5],[6,7],[8,10].
```
NOTE: input types have been changed on April 15, 2019. Please reset to default code definition to get new method signature.

Solution:
```cpp
class Solution {
public:
    vector<vector<int>> insert(vector<vector<int>>& intervals, vector<int>& newInterval) {
        
    }
};
```

## 274. H-Index

Given an array of citations (each citation is a non-negative integer) of a researcher, write a function to compute the researcher's h-index.

According to the definition of h-index on Wikipedia: "A scientist has index h if h of his/her N papers have at least h citations each, and the other N − h papers have no more than h citations each."

Example:
```
Input: citations = [3,0,6,1,5]
Output: 3 
Explanation: [3,0,6,1,5] means the researcher has 5 papers in total and each of them had 
             received 3, 0, 6, 1, 5 citations respectively. 
             Since the researcher has 3 papers with at least 3 citations each and the remaining 
             two with no more than 3 citations each, her h-index is 3.
```             
Note: If there are several possible values for h, the maximum one is taken as the h-index.

Solution:
```cpp
class Solution {
public:
    int hIndex(vector<int>& citations) {
        
    }
};
```

## 1122. Relative Sort Array

Given two arrays arr1 and arr2, the elements of arr2 are distinct, and all elements in arr2 are also in arr1.

Sort the elements of arr1 such that the relative ordering of items in arr1 are the same as in arr2.  Elements that don't appear in arr2 should be placed at the end of arr1 in ascending order.

 

Example 1:
```
Input: arr1 = [2,3,1,3,2,4,6,7,9,2,19], arr2 = [2,1,4,3,9,6]
Output: [2,2,2,1,4,3,3,9,6,7,19]
```

Constraints:

- arr1.length, arr2.length <= 1000
- 0 <= arr1[i], arr2[i] <= 1000
- Each arr2[i] is distinct.
- Each arr2[i] is in arr1.

Solution:
```cpp
class Solution {
public:
    vector<int> relativeSortArray(vector<int>& arr1, vector<int>& arr2) {
        
    }
};
```

## 493. Reverse Pairs

Given an array nums, we call (i, j) an important reverse pair if i < j and nums[i] > 2*nums[j].

You need to return the number of important reverse pairs in the given array.

Example1:
```
Input: [1,3,2,3,1]
Output: 2
```
Example2:
```
Input: [2,4,3,5,1]
Output: 3
```
Note:
- The length of the given array will not exceed 50,000.
- All the numbers in the input array are in the range of 32-bit integer.

Solution:
```cpp
class Solution {
public:
    int reversePairs(vector<int>& nums) {
        
    }
};
```

## 252. Meeting Rooms

Given an array of meeting time intervals consisting of start and end times [[s1,e1],[s2,e2],...] (si < ei), determine if a person could attend all meetings.

Example 1:
```
Input: [[0,30],[5,10],[15,20]]
Output: false
```
Example 2:
```
Input: [[7,10],[2,4]]
Output: true
```
NOTE: input types have been changed on April 15, 2019. Please reset to default code definition to get new method signature.

Solution:
```cpp
class Solution {
public:
    bool canAttendMeetings(vector<vector<int>>& intervals) {
        
    }
};
```

## 1057. Campus Bikes

On a campus represented as a 2D grid, there are N workers and M bikes, with N <= M. Each worker and bike is a 2D coordinate on this grid.

Our goal is to assign a bike to each worker. Among the available bikes and workers, we choose the (worker, bike) pair with the shortest Manhattan distance between each other, and assign the bike to that worker. (If there are multiple (worker, bike) pairs with the same shortest Manhattan distance, we choose the pair with the smallest worker index; if there are multiple ways to do that, we choose the pair with the smallest bike index). We repeat this process until there are no available workers.

The Manhattan distance between two points p1 and p2 is Manhattan(p1, p2) = |p1.x - p2.x| + |p1.y - p2.y|.

Return a vector ans of length N, where ans[i] is the index (0-indexed) of the bike that the i-th worker is assigned to.

 

Example 1:

![](https://assets.leetcode.com/uploads/2019/03/06/1261_example_1_v2.png)

```
Input: workers = [[0,0],[2,1]], bikes = [[1,2],[3,3]]
Output: [1,0]
Explanation: 
Worker 1 grabs Bike 0 as they are closest (without ties), and 
Worker 0 is assigned Bike 1. So the output is [1, 0].
```

Example 2:

![](https://assets.leetcode.com/uploads/2019/03/06/1261_example_2_v2.png)

```
Input: workers = [[0,0],[1,1],[2,0]], bikes = [[1,0],[2,2],[2,1]]
Output: [0,2,1]
Explanation: 
Worker 0 grabs Bike 0 at first. Worker 1 and Worker 2 share the same distance to 
Bike 2, thus Worker 1 is assigned to Bike 2, and Worker 2 will take Bike 1. So
the output is [0,2,1].
``` 

Note:

- 0 <= workers[i][j], bikes[i][j] < 1000
- All worker and bike locations are distinct.
- 1 <= workers.length <= bikes.length <= 1000

Solution:
```cpp
class Solution {
public:
    vector<int> assignBikes(vector<vector<int>>& workers, vector<vector<int>>& bikes) {
        
    }
};
```

## 1152. Analyze User Website Visit Pattern

We are given some website visits: the user with name username[i] visited the website website[i] at time timestamp[i].

A 3-sequence is a list of websites of length 3 sorted in ascending order by the time of their visits.  (The websites in a 3-sequence are not necessarily distinct.)

Find the 3-sequence visited by the largest number of users. If there is more than one solution, return the lexicographically smallest such 3-sequence.

 

Example 1:
```
Input: username =
["joe","joe","joe","james","james","james","james","mary","mary","mary"], 

timestamp = [1,2,3,4,5,6,7,8,9,10], 

website = 
["home","about","career","home","cart","maps","home","home","about","career"]

Output: ["home","about","career"]

Explanation: 
The tuples in this example are:
["joe", 1, "home"]
["joe", 2, "about"]
["joe", 3, "career"]
["james", 4, "home"]
["james", 5, "cart"]
["james", 6, "maps"]
["james", 7, "home"]
["mary", 8, "home"]
["mary", 9, "about"]
["mary", 10, "career"]
The 3-sequence ("home", "about", "career") was visited at least once by 2 users.
The 3-sequence ("home", "cart", "maps") was visited at least once by 1 user.
The 3-sequence ("home", "cart", "home") was visited at least once by 1 user.
The 3-sequence ("home", "maps", "home") was visited at least once by 1 user.
The 3-sequence ("cart", "maps", "home") was visited at least once by 1 user.
``` 

Note:

- 3 <= N = username.length = timestamp.length = website.length <= 50
- 1 <= username[i].length <= 10
- 0 <= timestamp[i] <= 10^9
- 1 <= website[i].length <= 10
- Both username[i] and website[i] contain only lowercase characters.
- It is guaranteed that there is at least one user who visited at least 3 websites.
- No user visits two websites at the same time.

Solution:
```cpp
class Solution {
public:
    vector<string> mostVisitedPattern(vector<string>& username, vector<int>& timestamp, vector<string>& website) {
        
    }
};
```
