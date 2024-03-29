## git版本

```shell
git -v
git --version
```

## linux系统操作指令

| **指令**      | **含义**                      | **说明**               |
| ----------- | --------------------------- | -------------------- |
| cd 目录       | change directory            | 改变操作目录               |
| cd ..       |                             | 退回到上一级目录             |
| pwd         | Print work<br> directory    | 打印工作目录               |
| ls          | list directory<br> contents | 显示当前目录的文件及子文件目录      |
| ll          | ls -l 简化版本                  | 更详细地显示当前目录的文件及子文件目录  |
| mkdir 文件夹名称 | make directory              | 新建一个文件夹              |
| rm 文件       | remove                      | 删除文件                 |
| rm -r 文件夹   | Remove                      | 删除文件目录               |
| touch 文件    |                             | 如果创建的文件不存在，那么创建一个空文件 |
| reset       |                             | 清屏                   |
| clear       |                             | 清屏                   |
| exit        |                             | 退出终端窗口               |

## 配置用户信息

```shell
git config --global user.name aztl
git config --global user.email emailaddress
```

## 查看git状态

`git status`

## 将文件添加到暂存区

`git add test.txt`

## 将文件放置在版本库中

`git commit -m "my first git file"`

将添加和放置合并成一步

`git commit -a -m "update file"`

## 从版本库中恢复文件

`git restore test.txt`  

## 查看版本库文件历史

`git log`

## 将版本库文件重置到某一个版本

`git reset --hard 版本号`

## 创建分支

```shell
git branch b1
git branch b2
```

## 查看分支

```shell
git branch -v
```

## 切换分支

`git checkout b1`

## 删除分支

`git branch -d b2`

## 创建分支并直接切换到新的分支

`get checkout -b 分支名称`

edit by aztl

## 合并分支

`git merge 分支名称`

## 查看当前所有远程地址别名

`git remote -v`

## 添加别名

`git remote add 别名 别名地址`

## 推送本地分支到远程仓库

一次只能推送一个**分支**

`git push 别名 分支`

## 拉取远程仓库到本地

`git pull 别名 分支`

## 克隆远程仓库到本地

`git clone 远程地址`

会自动创建别名

## 跨团队合作

用fork按钮

然后pull request

## Github SSH免密登录

在用户文件夹将`.ssh`文件夹删除，然后在git的终端中打开

输入

`ssh-keygen -t rsa -C emailaddress`

三下回车

将生成的公钥粘贴到github网站的setting->SSH and GPG keys

以后拉取的时候，直接用SSH
