## 目标
## Purpose
Python回溯算法，实现任意形状物品装入任意形状2D方格的装箱

Python backtracking algorithm to realize the bin packing of any shape items into any shape 2D squares
## 原理
## Principle
回溯遍历所有可装满的可能，返回装箱结果

Backtracking through all possible filling possibilities and return the result of bin packing.
## 用法
## Usage

### 输入
### Input

```
	# [[rows, cols, mat, amount], … ]
	input_packs = [[2,2,[1,0,1,1],2],[1,2,[1,1],2],[2,4,[1,1,1,1,1,0,0,0],1]]
	myboard = board(np.array([[1, 0, 0, 1, 1], [1, 0, 0, 0, 1], [0, 0, 0, 0, 0], [1, 1, 0, 0, 0]]), np.zeros((4, 5)))
```


### 输出
### Output

```
	# A list of solutions
	a = backtracking(myboard, pack_lists)
	print(len(a))
		
	# Display the first solution
	print(a[0].color_board)
	plot_mat(a[0].color_board)
```
颜色代表了插入块的种类，最大的插入块索引在前
The color represents the type of insert block, with the largest insert block index coming first.

![image](https://github.com/Jiayuan-Shi/Bin_packing_python/assets/51028227/9ad18b1f-2ff3-457f-8fb1-9863ff90b47b)


