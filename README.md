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
	input_packs = [[1, 3, [1, 1, 1], 2], [1, 4, [1, 1, 1, 1], 2], [2, 3, [1, 1, 1, 1, 1, 1], 1], [2, 2, [1, 1, 1, 1], 1]]
	myboard = board(np.zeros((4, 5)), np.zeros((4, 5)))
```


### 输出
### Output

```
	# A list of solutions
	a = backtracking(myboard, pack_lists)
	print(len(a))
		
	# Display first solution
	print(a[0].color_board)
	plot_mat(a[0].color_board)
```
![image](https://github.com/Jiayuan-Shi/Bin_packing_python/assets/51028227/dffd53d4-8bb6-44ff-aab2-71684939f8bb)

