# 栈和队列

## 简介

    栈的特点是后入先出，根据这个特点可以临时保存一些数据，之后用到依次再弹出来，常用于 DFS 深度搜索

    队列一般常用于 BFS 广度搜索，类似一层一层的搜索

## 知识点
    - 熟悉栈的使用场景
      - 后入先出，保存临时值
      - 利用栈 DFS 深度搜索

    - 熟悉队列的使用场景
      - 利用队列 BFS 广度搜索


## Stack 栈

[min-stack](https://leetcode-cn.com/problems/min-stack/)
    设计一个支持 push，pop，top 操作，并能在常数时间内检索到最小元素的栈。
    思路：用两个栈实现，一个最小栈始终保证最小值在顶部

    ```python
    pass

    ```

[evaluate-reverse-polish-notation](https://leetcode-cn.com/problems/evaluate-reverse-polish-notation/)
    **波兰表达式计算** > **输入:** `["2", "1", "+", "3", "*"]` > **输出:** 9
    **解释:** `((2 + 1) * 3) = 9`

    思路：通过栈保存原来的元素，遇到表达式弹出运算，再推入结果，重复这个过程

    ```python
    pass

    ```

[decode-string](https://leetcode-cn.com/problems/decode-string/)

    给定一个经过编码的字符串，返回它解码后的字符串。
    s = "3[a]2[bc]", 返回 "aaabcbc".
    s = "3[a2[c]]", 返回 "accaccacc".
    s = "2[abc]3[cd]ef", 返回 "abcabccdcdcdef".

    思路：通过栈辅助进行操作

    ```python
    pass

    ```

    利用栈进行 DFS 递归搜索模板

    ```python
    pass

    ```

[binary-tree-inorder-traversal](https://leetcode-cn.com/problems/binary-tree-inorder-traversal/)

    给定一个二叉树，返回它的*中序*遍历。


    ```python
    pass

    ```

[clone-graph](https://leetcode-cn.com/problems/clone-graph/)

    给你无向连通图中一个节点的引用，请你返回该图的深拷贝（克隆）。

    ```python
    pass

    ```

[number-of-islands](https://leetcode-cn.com/problems/number-of-islands/)

    给定一个由  '1'（陆地）和 '0'（水）组成的的二维网格，计算岛屿的数量。一个岛被水包围，并且它是通过水平方向或垂直方向上相邻的陆地连接而成的。你可以假设网格的四个边均被水包围。

    思路：通过深度搜索遍历可能性（注意标记已访问元素）

    ```python
    pass

    ```

[largest-rectangle-in-histogram](https://leetcode-cn.com/problems/largest-rectangle-in-histogram/)

    给定 _n_ 个非负整数，用来表示柱状图中各个柱子的高度。每个柱子彼此相邻，且宽度为 1 。
    求在该柱状图中，能够勾勒出来的矩形的最大面积。

    思路：求以当前柱子为高度的面积，即转化为寻找小于当前值的左右两边值


    用栈保存小于当前值的左的元素


    ```python
    pass

    ```

## Queue 队列

    常用于 BFS 宽度优先搜索

[implement-queue-using-stacks](https://leetcode-cn.com/problems/implement-queue-using-stacks/)

    使用栈实现队列

    ```python
    pass

    ```

二叉树层次遍历

    ```python
    pass

    ```

[01-matrix](https://leetcode-cn.com/problems/01-matrix/)

    给定一个由 0 和 1 组成的矩阵，找出每个元素到最近的 0 的距离。
    两个相邻元素间的距离为 1

    ```python
    pass

    ```


## 练习

- [min-stack](https://leetcode-cn.com/problems/min-stack/)
- [evaluate-reverse-polish-notation](https://leetcode-cn.com/problems/evaluate-reverse-polish-notation/)
- [decode-string](https://leetcode-cn.com/problems/decode-string/)
- [binary-tree-inorder-traversal](https://leetcode-cn.com/problems/binary-tree-inorder-traversal/)
- [clone-graph](https://leetcode-cn.com/problems/clone-graph/)
- [number-of-islands](https://leetcode-cn.com/problems/number-of-islands/)
- [largest-rectangle-in-histogram](https://leetcode-cn.com/problems/largest-rectangle-in-histogram/)
- [implement-queue-using-stacks](https://leetcode-cn.com/problems/implement-queue-using-stacks/)
- [01-matrix](https://leetcode-cn.com/problems/01-matrix/)
