# 撤销 commit
- `git reset --soft HEAD~1/HEAD^`：撤销最近一次 commit，修改还在暂存区
- `git reset --mixed HEAD~1/HEAD^`：撤销最近一次 commit，修改还在 disk 但是不在暂存区
- `git reset --hard HEAD~1/HEAD^`：撤销最近一次 commit，连同 disk 上的操作也一并撤销
- `git revert HEAD`：相当于撤销最近一次 commit，但是原理是往最新的 commit 上新增一个反作用 commit，即最新的如果是 +1，那么 revert 后就会 -1   

注意：revert 可以撤销提交中的任意一次提交，因为这是添加反作用，不是回退，所以可以抵消任意一次提交而不改变其他的

# 测试
- 测试 --soft
- 测试 --mixed
- 测试 --hard

+1
+2