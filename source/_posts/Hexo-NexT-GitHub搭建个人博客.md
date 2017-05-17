---
title: Hexo + NexT + GitHub搭建个人博客
date: 2017-05-17 16:20:27
tags:
---

# 一、使用[Hexo](https://hexo.io/)建站

### 新建网站

``` bash
$ hexo init [folder]
```

### 创建文章

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### 开启服务

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### 生成静态文件

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### 部署页面

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/deployment.html)

# 二、更换[NexT](http://theme-next.iissnan.com/)主题

### 下载主题

``` bash
$ cd your-hexo-site
$ git clone https://github.com/iissnan/hexo-theme-next themes/next
```

### 启用主题

修改项目配置文件_config.yml
``` bash
theme: next
```

# 三、部署到[GitHub](https://github.com/)

### 创建域名仓库

[username].github.io

### 上传静态文件

把项目public目录下的文件上传到域名仓库

### 配置个人域名

以阿里云为例：

1.进入域名解析页面，添加CNAME解析
``` bash
www -> [username].github.io
```

2.在域名仓库下添加CNAME配置文件
``` bash
www.[your_domain].me
```