# Lab 1 

## 教学团队
### 教师：郑骁庆
联系方式：[zhengxq@fudan.edu.cn](http://zhengxq@fudan.edu.cn)
### 助教：
- 陈雷远 [20210240034@fudan.edu.cn](http://20210240034@fudan.edu.cn) 
- 徐健涵 [20210240021@fudan.edu.cn](http://20210240021@fudan.edu.cn) 


## 任务

- 设计链表

- 三数之和问题求解

> 本节目标：
>
> 1. 掌握链表的简单实现
> 2. 学会计算算法的时间复杂度与空间复杂度
> 3. 尝试从算法复杂度角度优化算法

## 获取及提交lab

**获取**：通过 `https://github.com/2020-Data-structure-and-algorithm/lab1`，获取。

**提交**：待定

**提交物**：本课程要求使用java或python语言完成，本次lab如果用java语言完成需提交MyLinkedList.java 以及 ThreeSum.java；python语言以此类推

**截止时间**：2020年9月26日 23：59：59

## 1.设计链表
## #问题描述
设计链表的实现。您可以选择使用单链表或双链表。单链表中的节点应该具有两个属性：val 和 next。val 是当前节点的值，next 是指向下一个节点的指针/引用。如果要使用双向链表，则还需要一个属性 prev 以指示链表中的上一个节点。假设链表中的所有节点都是 0-index 的。

在链表类中实现这些功能：

get(index)：获取链表中第 index 个节点的值。如果索引无效，则返回-1。

addAtHead(val)：在链表的第一个元素之前添加一个值为 val 的节点。插入后，新节点将成为链表的第一个节点。

addAtTail(val)：将值为 val 的节点追加到链表的最后一个元素。

addAtIndex(index,val)：在链表中的第 index 个节点之前添加值为 val  的节点。如果 index 等于链表的长度，则该节点将附加到链表的末尾。如果 index 大于链表长度，则不会插入节点。如果index小于0，则在头部插入节点。

deleteAtIndex(index)：如果索引 index 有效，则删除链表中的第 index 个节点。
 

### 示例：
```
MyLinkedList linkedList = new MyLinkedList();

linkedList.addAtHead(1);

linkedList.addAtTail(3);

linkedList.addAtIndex(1,2);   //链表变为1-> 2-> 3

linkedList.get(1);            //返回2 

linkedList.deleteAtIndex(1);  //现在链表是1-> 3

linkedList.get(1);            //返回3
 ```

### 提示：

所有val值都在 [1, 1000] 之内。

操作次数将在  [1, 1000] 之内。

请不要使用内置的 LinkedList 库。

## 2.三数之和
### 问题描述
给你一个包含 n 个整数的数组 nums，判断 nums 中是否存在三个元素 a，b，c ，使得 a + b + c = 0 ？请你找出所有满足条件且不重复的三元组。

注意：答案中不可以包含重复的三元组。

 ### 示例：

给定数组 nums = [-1, 0, 1, 2, -1, -4]，

满足要求的三元组集合为：

[

  [-1, 0, 1],
  
  [-1, -1, 2]
  
]

### 注意：
计算下你实现的算法的时间复杂度与空间复杂度，思考有没有更优的解法（时间复杂度更低，占用空间更少的解法）