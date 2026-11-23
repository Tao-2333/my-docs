# Git 命令参考

本页面整理一些常用 Git 命令，方便在实际开发中快速查阅。

## 1. git clone

**作用：** 将远程仓库克隆到本地。

基本格式：

```bash
git clone <仓库地址>
```

示例：

```bash
git clone https://github.com/git/git.git
```

执行后，Git 会下载该仓库的项目文件及相关版本历史。

## 2. git log

**作用：** 查看当前分支可达的提交历史。

```bash
git log --oneline
```

其中 `--oneline` 用于以简洁形式显示提交记录。

## 3. git diff

**作用：** 比较文件内容之间的差异。

```bash
git diff
```

默认显示工作区与暂存区之间的差异。

如果想查看已经暂存但尚未提交的变化，可以使用：

```bash
git diff --staged
```

## 4. git branch

**作用：** 查看或管理分支。

```bash
git branch
```

查看本地分支。

```bash
git branch feature
```

创建名为 `feature` 的新分支，但不会自动切换。

## 5. 常用命令总结

| 命令 | 功能 |
| --- | --- |
| `git init` | 初始化仓库 |
| `git clone` | 克隆远程仓库 |
| `git status` | 查看文件状态 |
| `git add` | 添加文件到暂存区 |
| `git commit` | 创建提交 |
| `git push` | 推送到远程仓库 |
| `git pull` | 获取并整合远程更新 |
| `git log` | 查看提交历史 |
| `git diff` | 查看文件差异 |

## 总结

Git 命令看起来很多，但日常使用只需要先熟悉其中一部分。

比起单纯记忆命令，我认为理解各个命令操作的对象，以及它们如何影响工作区、暂存区和仓库，更有助于掌握 Git。

[返回首页](index.md) | [查看使用指南](guide.md)