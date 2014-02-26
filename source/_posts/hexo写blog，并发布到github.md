title: 使用hexo写Blog，并发布到github
date: 2014-02-26 09:26:35
tags: [hexo]
---

##安装nodejs

> 1. 下载[nodejs](http://nodejs.org/download/)，选择对应的操作系统版本。
> 2. 安装，一路next。 
> 3. 打开cmd窗口，输入： node -v 
> 4. 正确显示nodejs的版本号，即安装成功。

##安装hexo

> 安装hexo，根据网络状况需要一定的时间
```
> npm install hexo -g
```
> 初始化blog.
```
> $ hexo init blog && cd blog
```
> 创建blog文章
```
> $ hexo new "Hello World"
```
> 启动服务器,输入：http://localhost:4000 访问之.
```
> $ hexo server
```
> 安装主题，hexo主题列表： [Themes](https://github.com/tommy351/hexo/wiki/Themes)
```
cd %BLOG_PATH
$ git clone <repository> themes/<theme-name>
```

##部署到github
> 1. 下载安装[git](https://code.google.com/p/msysgit/downloads/list)。
> 2. 在github申请账号，并创建一个username.github.io的仓库名（username为你的账号名）.
> 3. 根据github官方帮助文档,[安装SSH KEYS](https://help.github.com/articles/generating-ssh-keys)
> 4. 进入上述的blog目录，打开_config.yml文件，修改deploy段配置，详见：[Hexo Deployment](http://zespia.tw/hexo/docs/deployment.html)
> 5. 部署到github
```
hexo deploy --或者 hexo d
```

##参考
> http://ibruce.info/2013/11/22/hexo-your-blog/