# 进行一次编辑
- `git add .`：添加到本地
- `git diff`：查看本地上次 add 和未 add 的修改
- `git diff HEAD`：查看与上次提交相比的变化
- `git status`：查看文件的状态

<br/>  

# 撤销本地的修改
- `git status`：先查看本地提交的文件，方便下一步撤销
- `git checkout/restore --staged <change_file>`：撤销本地指定文件的修改（有些版本不能用 checkout）
