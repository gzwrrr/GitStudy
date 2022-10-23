# 进行一次编辑
- `git add .`：添加到本地
- `git diff`：查看本地上次 add 和未 add 的修改
- `git diff HEAD`：查看与上次提交相比的变化
- `git status`：查看文件的状态

<br/>  

# 撤销本地的修改
- `git status`：先查看本地提交的文件，方便下一步撤销
- `git restore --staged <change_file>`：撤销本地指定文件的修改，但是会保留磁盘上的操作，比较安全，执行后文件是未 add 的状态，即移出暂存区
- `git checkout HEAD <change_file>`：撤销本地文件的修改到上一次提交的状态，不会保留磁盘上的操作，很危险