# 二分搜索

## 二分搜索模板
    给一个**有序数组**和目标值，找第一次/最后一次/任何一次出现的索引，如果没有出现返回-1

模板四点要素
    - 1、初始化：start=0、end=len-1
    - 2、循环退出条件：start + 1 < end
    - 3、比较中点和目标值：A[mid] ==、 <、> target
    - 4、判断最后两个元素是否符合：A[start]、A[end] ? target

    时间复杂度 O(logn)，使用场景一般是有序数组的查找

## 知识点
    二分搜索核心四点要素（必背&理解）

    - 1、初始化：start=0、end=len-1
    - 2、循环退出条件：start + 1 < end
    - 3、比较中点和目标值：A[mid] ==、 <、> target
    -4、判断最后两个元素是否符合：A[start]、A[end] ? target


典型示例

[binary-search](https://leetcode-cn.com/problems/binary-search/)
给定一个  n  个元素有序的（升序）整型数组  nums 和一个目标值  target  ，写一个函数搜索  nums  中的 target，如果目标值存在返回下标，否则返回 -1。

    ```
    pass
    ```

    大部分二分查找类的题目都可以用这个模板，然后做一点特殊逻辑即可

    另外二分查找还有一些其他模板如下图，大部分场景模板#3 都能解决问题，而且还能找第一次/最后一次出现的位置，应用更加广泛

![binary_search_template](https://img.fuiboom.com/img/binary_search_template.png)

    所以用模板#3 就对了，详细的对比可以这边文章介绍：[二分搜索模板](https://leetcode-cn.com/explore/learn/card/binary-search/212/template-analysis/847/)

    如果是最简单的二分搜索，不需要找第一个、最后一个位置、或者是没有重复元素，可以使用模板#1，代码更简洁
    ```
    pass
    ```


## 常见题目

### [search-for-range](https://www.lintcode.com/problem/search-for-a-range/description)

    给定一个包含 n 个整数的排序数组，找出给定目标值 target 的起始和结束位置。
    如果目标值不在数组中，则返回`[-1, -1]`

    思路：核心点就是找第一个 target 的索引，和最后一个 target 的索引，所以用两次二分搜索分别找第一次和最后一次的位置

    ```
    pass
    ```


### [search-insert-position](https://leetcode-cn.com/problems/search-insert-position/)
    给定一个排序数组和一个目标值，在数组中找到目标值，并返回其索引。如果目标值不存在于数组中，返回它将会被按顺序插入的位置。

    ```
    pass
    ```

### [search-a-2d-matrix](https://leetcode-cn.com/problems/search-a-2d-matrix/)

    编写一个高效的算法来判断  m x n  矩阵中，是否存在一个目标值。该矩阵具有如下特性：

    - 每行中的整数从左到右按升序排列。
    - 每行的第一个整数大于前一行的最后一个整数。

    ```
    pass
    ```

### [first-bad-version](https://leetcode-cn.com/problems/first-bad-version/)

    假设你有 n 个版本 [1, 2, ..., n]，你想找出导致之后所有版本出错的第一个错误的版本。
    你可以通过调用  bool isBadVersion(version)  接口来判断版本号 version 是否在单元测试中出错。实现一个函数来查找第一个错误的版本。你应该尽量减少对调用 API 的次数。

    ```
    pass
    ```

### [find-minimum-in-rotated-sorted-array](https://leetcode-cn.com/problems/find-minimum-in-rotated-sorted-array/)

    假设按照升序排序的数组在预先未知的某个点上进行了旋转( 例如，数组  [0,1,2,4,5,6,7] 可能变为  [4,5,6,7,0,1,2] )。
    请找出其中最小的元素。

    ```
    pass
    ```

### [find-minimum-in-rotated-sorted-array-ii](https://leetcode-cn.com/problems/find-minimum-in-rotated-sorted-array-ii/)

    假设按照升序排序的数组在预先未知的某个点上进行了旋转
    ( 例如，数组  [0,1,2,4,5,6,7] 可能变为  [4,5,6,7,0,1,2] )。
    请找出其中最小的元素。(包含重复元素)
    ```
    pass
    ```

### [search-in-rotated-sorted-array](https://leetcode-cn.com/problems/search-in-rotated-sorted-array/)

    假设按照升序排序的数组在预先未知的某个点上进行了旋转。
    ( 例如，数组  [0,1,2,4,5,6,7]  可能变为  [4,5,6,7,0,1,2] )。
    搜索一个给定的目标值，如果数组中存在这个目标值，则返回它的索引，否则返回  -1 。
    你可以假设数组中不存在重复的元素。

    ```
    pass
    ```

    注意点

    > 面试时，可以直接画图进行辅助说明，空讲很容易让大家都比较蒙圈

### [search-in-rotated-sorted-array-ii](https://leetcode-cn.com/problems/search-in-rotated-sorted-array-ii/)

    假设按照升序排序的数组在预先未知的某个点上进行了旋转。
    ( 例如，数组  [0,0,1,2,2,5,6]  可能变为  [2,5,6,0,0,1,2] )。
    编写一个函数来判断给定的目标值是否存在于数组中。若存在返回  true，否则返回  false。(包含重复元素)
    ```
    pass
    ```


## 练习题

- [search-for-range](https://www.lintcode.com/problem/search-for-a-range/description)
- [search-insert-position](https://leetcode-cn.com/problems/search-insert-position/)
- [search-a-2d-matrix](https://leetcode-cn.com/problems/search-a-2d-matrix/)
- [first-bad-version](https://leetcode-cn.com/problems/first-bad-version/)
- [find-minimum-in-rotated-sorted-array](https://leetcode-cn.com/problems/find-minimum-in-rotated-sorted-array/)
- [find-minimum-in-rotated-sorted-array-ii](https://leetcode-cn.com/problems/find-minimum-in-rotated-sorted-array-ii/)
- [search-in-rotated-sorted-array](https://leetcode-cn.com/problems/search-in-rotated-sorted-array/)
- [search-in-rotated-sorted-array-ii](https://leetcode-cn.com/problems/search-in-rotated-sorted-array-ii/)
