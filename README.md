这个项目是github page的生成程序
你能看到这个README.md文件是因为本分支不是master分支
而是hexo分支,hexo分支也是源代码分支,master分支存放的是本分支生成的文件
即当使用 hexo deploy 时更新的是master分支

###目录用途
```text

node_modules: 依赖包
public：存放生成的页面
scaffolds：生成文章的一些模板
source：用来存放你的文章
themes：主题
** _config.yml: 博客的配置文件**
.deploy_git: 存放使用hexo deploy时上传到github master的分支的文件

```


[hexo主题](https://hexo.io/themes/)

当添加新页面时,通过命令部署到github page

```shell script

hexo clean
hexo generate
hexo deploy

```

>其中 hexo clean清除了你之前生成的东西，也可以不加。
 hexo generate 顾名思义，生成静态文章，可以用 hexo g缩写
 hexo deploy 部署文章，可以用hexo d缩写,注意deploy时可能
>要你输入github的username和password。