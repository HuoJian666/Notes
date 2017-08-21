# Git reset命令整理
## Git reset  
Git reset会改变commit提交记录(git hi -5)，因为改变了HEAD  
三个概念：  
- **HEAD**：当前分支你最新commit的别名  
- **index**：也被称为staging area，暂存区  
- **Working Directory**：工作目录

Git reset有三个参数:**--mixed（默认参数），--soft，--hard**
- **--mixed参数**  
	默认是mixed参数：会将HEAD重置到reset指定的那个commit，index和HEAD同步，工作目录不发生变化。  
- **--soft参数**  
	HEAD重置，index不发生改变，工作目录不发生改变  
- **--hard参数**  
	HEAD重置，index和工作目录都和HEAD一致

**git reset +哈希值  将HEAD重置到这个哈希值的commit上**
**Git reset本质就是重置HEAD(当前分支的版本顶端）到另外一个commit**  
  
