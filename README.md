# 2
## 目录

#### 目录

#### 代码块

	while (Priosity(sTop) >= Priosity(head->getLex()))
			/*如果操作符栈顶运算符的优先级高于或等于当前读到的操作符*/
		{
			TreeNode *t = op_stack.pop();
			TreeNode *Rnum = num_stack.pop();
			TreeNode *Lnum = num_stack.pop();
			t->child[1] = Rnum;
			t->child[0] = Lnum;
			num_stack.push(t);
	
			sTop = op_stack.top()->attr.ExpAttr.op;
		}

----------
**粗体**
*斜体*
### [https://www.baidu.com/](https://www.baidu.com/ "百度")
#### ~~像这样~~



> 引用


> 1


> 2


> 3


> 1. a


> 2. b

| 1    | 2    | 3    |
| ---- | ---- | ---- |
| a    | a    | a    |
| b    | b    | b    |
| b    | b    | b    |


![image](https://github.com/iNoFound/2/blob/main/a1.png)
