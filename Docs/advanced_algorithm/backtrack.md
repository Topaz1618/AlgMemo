# 回溯法

## 背景

    回溯法（backtrack）常用于遍历列表所有子集，是 DFS 深度搜索一种，一般用于全排列，穷尽所有可能，遍历的过程实际上是一个决策树的遍历过程。时间复杂度一般 O(N!)，它不像动态规划存在重叠子问题可以优化，回溯算法就是纯暴力穷举，复杂度一般都很高。

## 模板

    ```
    pass
    ```

    核心就是从选择列表里做一个选择，然后一直递归往下搜索答案，如果遇到路径不通，就返回来撤销这次选择。

## 示例

### [subsets](https://leetcode-cn.com/problems/subsets/)

    > 给定一组不含重复元素的整数数组 nums，返回该数组所有可能的子集（幂集）。
    ```
    pass
    ```

### [subsets-ii](https://leetcode-cn.com/problems/subsets-ii/)

    > 给定一个可能包含重复元素的整数数组 nums，返回该数组所有可能的子集（幂集）。说明：解集不能包含重复的子集。

    ```
    pass
    ```

### [permutations](https://leetcode-cn.com/problems/permutations/)

    > 给定一个   没有重复   数字的序列，返回其所有可能的全排列。

    思路：需要记录已经选择过的元素，满足条件的结果才进行返回

    ```
    pass
    ```

### [permutations-ii](https://leetcode-cn.com/problems/permutations-ii/)

    > 给定一个可包含重复数字的序列，返回所有不重复的全排列。

    ```
    pass
    ```

## 练习

- [subsets](https://leetcode-cn.com/problems/subsets/)
- [subsets-ii](https://leetcode-cn.com/problems/subsets-ii/)
- [permutations](https://leetcode-cn.com/problems/permutations/)
- [permutations-ii](https://leetcode-cn.com/problems/permutations-ii/)

挑战题目

- [combination-sum](https://leetcode-cn.com/problems/combination-sum/)
- [letter-combinations-of-a-phone-number](https://leetcode-cn.com/problems/letter-combinations-of-a-phone-number/)
- [palindrome-partitioning](https://leetcode-cn.com/problems/palindrome-partitioning/)
- [restore-ip-addresses](https://leetcode-cn.com/problems/restore-ip-addresses/)
- [permutations](https://leetcode-cn.com/problems/permutations/)
