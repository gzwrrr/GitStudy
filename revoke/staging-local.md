# 撤销 commit
- `git reset --soft HEAD~1/HEAD^`：撤销最近一次 commit，修改还在暂存区
- `git reset --mixed HEAD~1/HEAD^`：撤销最近一次 commit，修改还在 disk 但是不在暂存区
- `git reset --hard HEAD~1/HEAD^`：撤销最近一次 commit，连同 disk 上的操作也一并撤销
- `git revert HEAD`：加一个最新 commit 的反作用 commit，即如果上一次 commit 是 +1，那么 revert 后就是 -1

# 测试
- 测试 --soft
- 测试 --mixed
- 测试 --hard
- 测试 revert