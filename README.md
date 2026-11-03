# git-practice

Git 练习仓库，用于熟悉日常 Git 工作流。

## 常用命令速查

```bash
# 查看状态与历史
git status                 # 工作区/暂存区状态
git log --oneline --graph  # 图形化提交历史
git diff                   # 未暂存的改动
git diff --staged          # 已暂存的改动

# 提交
git add <file>             # 暂存指定文件
git add -A                 # 暂存全部改动
git commit -m "message"    # 提交

# 分支
git branch                 # 列出本地分支
git switch -c <name>       # 新建并切换分支（推荐）
git switch main            # 切换分支
git merge <name>           # 合并分支

# 远程
git remote -v              # 查看远程地址
git fetch origin           # 拉取远程更新（不合并）
git pull --rebase          # 拉取并变基
git push -u origin main    # 首次推送并建立追踪
```

## 分支约定

- `main`：主分支，保持可用
- 其他分支：按功能/练习目的命名，如 `feature/xxx`、`practice/xxx`
