# 二叉树
## 树的构建
基于ListNode结构，有本节点值，做有节点对象

二叉树是每个节点最多有两个节点的树结构。

root, parent node, child node, siblings, leaf, sub-tree

``` java
树的定义：

Public class TreeNode {

​	public int val;	

​	public TreeNode left,  right;

​	public TreeNode(int val) {

​	This.val = val;

​	}

}  
```  
平衡二叉树 Balanced Binary Tree

1.可以是一颗空树

2.左右子树高度之差不大于1

3.子树也必须是一颗平衡二叉树



二叉树的种类

空二叉树

退化二叉树：Degenerate;只有一条线。

完全二叉树：Complete; 左半边完整 右边缺失；

满二叉树：Full; 任何一个节点 要么有两个孩子 要么没有孩子

完美二叉树：Perfect 任何一个Parent node 都有两个孩子， 

平衡二叉树；

树是没有环的图
## 二叉树的宽度和深度优先遍历
Binary Tree BFS/DFS

### Binary Tree Breadth First Search(BFS) 二叉树宽度优先搜索

逐层优先遍历

从左到右。queue 来实现 offer/pull

时间复杂度  O(n)
空间复杂度  O(n) 由n个节点构成的二叉树，一层最多节点的个数为 (n+1)/2

### 分层遍历


### Binary Tree Depth First Search(DFS) 二叉树深度优先搜索
优先遍历最深的那一个节点

递归实现

preoder

inoder 

postoder 

时间复杂度  O(2n+1) n+1次null  +  n个节点
空间复杂度  
complete tree  
h = log(n+1);

degenerate tree
h = n;

因此空间复杂度为 O(n) ~ O(logn)

 
