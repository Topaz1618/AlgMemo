# 滑动窗口

## 总结
    - 和双指针题目类似，更像双指针的升级版，滑动窗口核心点是维护一个窗口集，根据窗口集来进行处理
    - 核心步骤
      - right 右移
      - 收缩
      - left 右移
      - 求结果


## 模板

    ```
    pass
    ```

    需要变化的地方

    - 1、右指针右移之后窗口数据更新
    - 2、判断窗口是否要收缩
    - 3、左指针右移之后窗口数据更新
    - 4、根据题意计算结果

## 示例

[minimum-window-substring](https://leetcode-cn.com/problems/minimum-window-substring/)

    > 给你一个字符串 S、一个字符串 T，请在字符串 S 里面找出：包含 T 所有字母的最小子串

    ```
    pass
    ```

[permutation-in-string](https://leetcode-cn.com/problems/permutation-in-string/)

    > 给定两个字符串  **s1**  和  **s2**，写一个函数来判断  **s2**  是否包含  **s1 **的排列。

    ```
    pass
    ```

[find-all-anagrams-in-a-string](https://leetcode-cn.com/problems/find-all-anagrams-in-a-string/)

    > 给定一个字符串  **s **和一个非空字符串  **p**，找到  **s **中所有是  **p **的字母异位词的子串，返回这些子串的起始索引。

    ```
    pass
    ```

[longest-substring-without-repeating-characters](https://leetcode-cn.com/problems/longest-substring-without-repeating-characters/)

    > 给定一个字符串，请你找出其中不含有重复字符的   最长子串   的长度。
    > 示例  1:
    >
    > 输入: "abcabcbb"
    > 输出: 3
    > 解释: 因为无重复字符的最长子串是 "abc"，所以其长度为 3。

    ```
    pass
    ```


## 练习

- [minimum-window-substring](https://leetcode-cn.com/problems/minimum-window-substring/)
- [permutation-in-string](https://leetcode-cn.com/problems/permutation-in-string/)
- [find-all-anagrams-in-a-string](https://leetcode-cn.com/problems/find-all-anagrams-in-a-string/)
- [longest-substring-without-repeating-characters](https://leetcode-cn.com/problems/longest-substring-without-repeating-characters/)
