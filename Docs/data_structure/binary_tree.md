# 二叉树

## 知识点
    - 掌握二叉树递归与非递归遍历
    - 理解 DFS 前序遍历与分治法
    - 理解 BFS 层次遍历

### 二叉树遍历
    **前序遍历**：**先访问根节点**，再前序遍历左子树，再前序遍历右子树
    **中序遍历**：先中序遍历左子树，**再访问根节点**，再中序遍历右子树
    **后序遍历**：先后序遍历左子树，再后序遍历右子树，**再访问根节点**

注意点
    - 以根访问顺序决定是什么遍历
    - 左子树都是优先右子树

#### 前序递归
    ``` python
    pass
    ```

#### 前序非递归
    ``` python
    pass
    ```


#### 中序非递归
    ``` python
    pass
    ```


#### 后序非递归
    ``` python
    pass
    ```

    注意点
    - 核心就是：根节点必须在右节点弹出之后，再弹出

#### DFS 深度搜索-从上到下

    ``` python
    pass
    ```


#### DFS 深度搜索-从下向上（分治法）
    ``` python
    pass
    ```

    注意点：
    DFS 深度搜索（从上到下） 和分治法区别：前者一般将最终结果通过指针参数传入，后者一般递归返回结果最后合并

#### BFS 层次遍历
    ``` python
    pass
    ```



### 分治法应用

    先分别处理局部，再合并结果

    适用场景
    - 快速排序
    - 归并排序
    - 二叉树相关问题

    分治法模板
    - 递归返回条件
    - 分段处理
    - 合并结果

    ``` python
    pass
    ```


#### 归并排序  
    ``` python
    pass
    ```

    注意点
    递归需要返回结果用于合并

#### 快速排序  
    ``` python
    pass
    ```

    注意点：
        快排由于是原地交换所以没有合并过程
        传入的索引是存在的索引（如：0、length-1 等），越界可能导致崩溃


常见题目示例

#### maximum-depth-of-binary-tree
[maximum-depth-of-binary-tree](https://leetcode-cn.com/problems/maximum-depth-of-binary-tree/)

    给定一个二叉树，找出其最大深度。

    思路：分治法

    ``` python
    pass
    ```


#### balanced-binary-tree

[balanced-binary-tree](https://leetcode-cn.com/problems/balanced-binary-tree/)

    给定一个二叉树，判断它是否是高度平衡的二叉树。

    思路：分治法，左边平衡 && 右边平衡 && 左右两边高度 <= 1，
    因为需要返回是否平衡及高度，要么返回两个数据，要么合并两个数据，
    所以用-1 表示不平衡，>0 表示树高度（二义性：一个变量有两种含义）。

    ``` python
    pass
    ```

    注意
    一般工程中，结果通过两个变量来返回，不建议用一个变量表示两种含义


#### binary-tree-maximum-path-sum
[binary-tree-maximum-path-sum](https://leetcode-cn.com/problems/binary-tree-maximum-path-sum/)

    给定一个**非空**二叉树，返回其最大路径和。

    思路：分治法，分为三种情况：左子树最大路径和最大，右子树最大路径和最大，左右子树最大加根节点最大，需要保存两个变量：一个保存子树最大路径和，一个保存左右加根节点和，然后比较这个两个变量选择最大值即可

    ``` python
    pass
    ```

#### lowest-common-ancestor-of-a-binary-tree
[lowest-common-ancestor-of-a-binary-tree](https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-tree/)
    给定一个二叉树, 找到该树中两个指定节点的最近公共祖先。
    思路：分治法，有左子树的公共祖先或者有右子树的公共祖先，就返回子树的祖先，否则返回根节点

    ``` python
    pass
    ```


### BFS 层次应用
#### binary-tree-level-order-traversal

[binary-tree-level-order-traversal](https://leetcode-cn.com/problems/binary-tree-level-order-traversal/)
    给你一个二叉树，请你返回其按  **层序遍历**  得到的节点值。 （即逐层地，从左到右访问所有节点）
    思路：用一个队列记录一层的元素，然后扫描这一层元素添加下一层元素到队列（一个数进去出来一次，所以复杂度 O(logN)）

    ``` python
    pass
    ```


#### binary-tree-level-order-traversal-ii
[binary-tree-level-order-traversal-ii](https://leetcode-cn.com/problems/binary-tree-level-order-traversal-ii/)
    给定一个二叉树，返回其节点值自底向上的层次遍历。 （即按从叶子节点所在层到根节点所在的层，逐层从左向右遍历）
    思路：在层级遍历的基础上，翻转一下结果即可

    ``` python
    pass
    ```



#### binary-tree-zigzag-level-order-traversal
[binary-tree-zigzag-level-order-traversal](https://leetcode-cn.com/problems/binary-tree-zigzag-level-order-traversal/)
    给定一个二叉树，返回其节点值的锯齿形层次遍历。Z 字形遍历

    ``` python
    pass
    ```


### 二叉搜索树应用
#### validate-binary-search-tree
[validate-binary-search-tree](https://leetcode-cn.com/problems/validate-binary-search-tree/)
    给定一个二叉树，判断其是否是一个有效的二叉搜索树。
    思路 1：中序遍历，检查结果列表是否已经有序
    思路 2：分治法，判断左 MAX < 根 < 右 MIN

    ``` python
    pass
    ```

#### insert-into-a-binary-search-tree
[insert-into-a-binary-search-tree](https://leetcode-cn.com/problems/insert-into-a-binary-search-tree/)
    给定二叉搜索树（BST）的根节点和要插入树中的值，将值插入二叉搜索树。 返回插入后二叉搜索树的根节点。
    思路：找到最后一个叶子节点满足插入条件即可

    ``` python
    pass
    ```


## 练习
- [maximum-depth-of-binary-tree](https://leetcode-cn.com/problems/maximum-depth-of-binary-tree/)
- [balanced-binary-tree](https://leetcode-cn.com/problems/balanced-binary-tree/)
- [binary-tree-maximum-path-sum](https://leetcode-cn.com/problems/binary-tree-maximum-path-sum/)
- [lowest-common-ancestor-of-a-binary-tree](https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-tree/)
- [binary-tree-level-order-traversal](https://leetcode-cn.com/problems/binary-tree-level-order-traversal/)
- [binary-tree-level-order-traversal-ii](https://leetcode-cn.com/problems/binary-tree-level-order-traversal-ii/)
- [binary-tree-zigzag-level-order-traversal](https://leetcode-cn.com/problems/binary-tree-zigzag-level-order-traversal/)
- [validate-binary-search-tree](https://leetcode-cn.com/problems/validate-binary-search-tree/)
- [insert-into-a-binary-search-tree](https://leetcode-cn.com/problems/insert-into-a-binary-search-tree/)
