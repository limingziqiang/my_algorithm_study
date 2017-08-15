### my_algorithm_study

[实现文章内容](http://www.jianshu.com/p/7e6589306a27)

[掘金文章](https://juejin.im/post/594dfe795188250d725a220a)

### 数据结构

* 栈：先入后出
* 队列：先入先出
* 字典：Object
* 链表：存储有序的元素结构，类似数组，在内存不连续放置;
* 集合：由一组无序且唯一的项组成;
* 散列：根据(key/value)直接进行访问的数据结构;他通过把关键码值映射到表中一个位置来访问记录，以加快查找的速度；这个映射函数叫散列函数，存放记录的数组叫散列表;
* 树：由n(n>=1)个有限节点组成有层次关系的集合;
```
二叉树中的节点最多只能有两个子节点：一个是左侧子节点，另一个是右侧子节点。
`二叉搜索树(BST)`：只允许你在左侧节点存储（比父节点）小的值， 在右侧节点存储（比父节点）大（或者等于）的值。
中序遍历：从最小到最大的顺序访问所有节点
先序遍历：以优先于后代节点的顺序访问每个节点的。（打印一个结构化的文档）
后序遍历：先访问节点的后代节点，再访问节点本身。（计算一个目录和它的子目录中所有文件所占空间的大小）
AVL树/红黑树
```
* 图：图是网络结构的抽象模型，任何二元关系都可以用图表示; 道路图、关系图; 呈多对多关系;

### 算法

- 冒泡排序 O(n²)

```
function bubbleSort(arr) {
	for(let i=0;i<arr.length;i++){
		for(let j=0;j<arr.length;j++){
			if(arr[j] > arr[i]){
				let tmp = arr[i]
				arr[i] = arr[j]
				arr[j] = tmp
			}
		}
	}
}
```

- 选择排序 
> 思路是找到最小的放第一位，第二小的第二位，依次类推

```

function selectSort(arr) {
	let minIndex
	for(let i=0;i<arr.length-1;i++){
		minIndex = i
		for(let j=i;j<arr.length;j++){
			if(arr[minIndex] > arr[j]){
				minIndex = j
			}
		}
		if(i !== minIndex){
			let tmp = arr[i]
			arr[i] = arr[minIndex]
			arr[minIndex] = tmp
		}
	}
}
```

- 插入排序
> 

- 归并排序 O(nlog^n)
> 递归把数组分为两个子数组，一直递归到数组中只有一个元素，然后调用函数把两个子数组排序，最后两数组合并

- 快速排序
> 








