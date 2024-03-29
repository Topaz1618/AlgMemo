# 链表

## 知识点
链表必须要掌握的一些点，通过下面练习题，基本大部分的链表类的题目都是手到擒来~
- null/nil 异常处理
- dummy node 哑巴节点
- 快慢指针
- 插入一个节点到排序链表
- 从一个链表中移除一个节点
- 翻转链表
- 合并两个链表
- 找到链表的中间节点

## Note
哑巴节点使用场景
> 当头节点不确定的时候，使用哑巴节点


## 常见题型

### [remove-duplicates-from-sorted-list](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list/)
    给定一个排序链表，删除所有重复的元素，使得每个元素只出现一次。

   ```
    pass
   ```
### [remove-duplicates-from-sorted-list-ii](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list-ii/)
    给定一个排序链表，删除所有含有重复数字的节点，只保留原始链表中   没有重复出现的数字。
    思路：链表头结点可能被删除，所以用 dummy node 辅助删除

   ```
    pass
   ```


### [reverse-linked-list](https://leetcode-cn.com/problems/reverse-linked-list/)
    反转一个单链表。

    思路：用一个 prev 节点保存向前指针，temp 保存向后的临时指针

   ```
    pass
   ```


### [reverse-linked-list-ii](https://leetcode-cn.com/problems/reverse-linked-list-ii/)
    反转从位置  *m*  到  *n*  的链表。请使用一趟扫描完成反转。

    思路：先遍历到 m 处，翻转，再拼接后续，注意指针处理

   ```
    pass
   ```


### [merge-two-sorted-lists](https://leetcode-cn.com/problems/merge-two-sorted-lists/)
    将两个升序链表合并为一个新的升序链表并返回。新链表是通过拼接给定的两个链表的所有节点组成的。

    思路：通过 dummy node 链表，连接各个元素
   ```
    pass
   ```



### [partition-list](https://leetcode-cn.com/problems/partition-list/)
    给定一个链表和一个特定值 x，对链表进行分隔，使得所有小于  *x*  的节点都在大于或等于  *x*  的节点之前。

    思路：将大于 x 的节点，放到另外一个链表，最后连接这两个链表

   ```
    pass
   ```


### [sort-list](https://leetcode-cn.com/problems/sort-list/)

    在  *O*(*n* log *n*) 时间复杂度和常数级空间复杂度下，对链表进行排序。

    思路：归并排序，找中点和合并操作

   ```
    pass
   ```


    注意点

        - 快慢指针 判断 fast 及 fast.Next 是否为 nil 值
        - 递归 mergeSort 需要断开中间节点
        - 递归返回条件为 head 为 nil 或者 head.Next 为 nil

### [reorder-list](https://leetcode-cn.com/problems/reorder-list/)
    给定一个单链表  *L*：*L*→*L*→…→*L\_\_n*→*L*
    将其重新排列后变为： *L*→*L\_\_n*→*L*→*L\_\_n*→*L*→*L\_\_n*→…

    思路：找到中点断开，翻转后面部分，然后合并前后两个链表


   ```
    pass
   ```

### [linked-list-cycle](https://leetcode-cn.com/problems/linked-list-cycle/)

    给定一个链表，判断链表中是否有环。

    思路：快慢指针，快慢指针相同则有环，证明：如果有环每走一步快慢指针距离会减 1
    ![fast_slow_linked_list](https://img.fuiboom.com/img/fast_slow_linked_list.png)


   ```
    pass
   ```

### [linked-list-cycle-ii](https://leetcode-cn.com/problems/linked-list-cycle-ii/)

    给定一个链表，返回链表开始入环的第一个节点。  如果链表无环，则返回  `null`。

    思路：快慢指针，快慢相遇之后，慢指针回到头，快慢指针步调一致一起移动，相遇点即为入环点
    ![cycled_linked_list](https://img.fuiboom.com/img/cycled_linked_list.png)


   ```
    pass
   ```

    坑点
    - 指针比较时直接比较对象，不要用值比较，链表中有可能存在重复值情况
    - 第一次相交后，快指针需要从下一个节点开始和头指针一起匀速移动

    另外一种方式是 fast=head,slow=head


   ```
    pass
   ```

    这两种方式不同点在于，**一般用 fast=head.Next 较多**，因为这样可以知道中点的上一个节点，可以用来删除等操作。

    - fast 如果初始化为 head.Next 则中点在 slow.Next
    - fast 初始化为 head,则中点在 slow

### [palindrome-linked-list](https://leetcode-cn.com/problems/palindrome-linked-list/)
    请判断一个链表是否为回文链表。
   ```
    pass
   ```

### [copy-list-with-random-pointer](https://leetcode-cn.com/problems/copy-list-with-random-pointer/)

    给定一个链表，每个节点包含一个额外增加的随机指针，该指针可以指向链表中的任何节点或空节点。
    要求返回这个链表的 深拷贝。

    思路：1、hash 表存储指针，2、复制节点跟在原节点后面

   ```
    pass
   ```



## 练习
- [remove-duplicates-from-sorted-list](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list/)
- [remove-duplicates-from-sorted-list-ii](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list-ii/)
- [reverse-linked-list](https://leetcode-cn.com/problems/reverse-linked-list/)
- [reverse-linked-list-ii](https://leetcode-cn.com/problems/reverse-linked-list-ii/)
- [merge-two-sorted-lists](https://leetcode-cn.com/problems/merge-two-sorted-lists/)
- [partition-list](https://leetcode-cn.com/problems/partition-list/)
- [sort-list](https://leetcode-cn.com/problems/sort-list/)
- [reorder-list](https://leetcode-cn.com/problems/reorder-list/)
- [linked-list-cycle](https://leetcode-cn.com/problems/linked-list-cycle/)
- [linked-list-cycle-ii](https://leetcode-cn.com/problems/linked-list-cycle-ii/)
- [palindrome-linked-list](https://leetcode-cn.com/problems/palindrome-linked-list/)
- [copy-list-with-random-pointer](https://leetcode-cn.com/problems/copy-list-with-random-pointer/)
