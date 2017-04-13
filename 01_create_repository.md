# 创建版本库

## git init

> 创建新的目录或者，选择已有的内容的目录执行 `git init` 命令即可

```
$ git init
Initialized empty Git repository in h:/github/learngit/.git/
```

瞬间Git就把仓库建好了,git会在当前目录下创建一个目录 `.git` 这个目录是存放版本跟踪的信息，千万不能动。

如果你没有看到`.git`目录，那是因为这个目录默认是隐藏的，用 `ls -a` 命令就可以看见。


## 把文件添加到版本库

`learngit`目录下（子目录也行）,创建 `readme.txt`

> * 第一步，用命令`git add`告诉Git，把文件添加到仓库
>
> ```
> $ git add readme.txt
> ```
>
> * 第二步，用命令`git commit`告诉Git，把文件提交到仓库
>
> ```
> $ git commit -m "wrote a readme file"
> [master (root-commit) cb926e7] wrote a readme file
> 1 file changed, 2 insertions(+)
> create mode 100644 readme.txt
> ```
>

**`git commit`命令，`-m`后面输入的是本次提交的说明**


## 小结

用`git init`来初始化一个Git仓库

添加文件到Git仓库，两步

 * 使用命令`git add <file>`，注意，可反复多次使用，添加多个文件
 * 使用命令`git commit`，完成提交



[参考资料](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/0013743256916071d599b3aed534aaab22a0db6c4e07fd0000)
