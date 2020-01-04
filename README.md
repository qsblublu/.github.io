# 模板地址

[GitHub 地址](https://github.com/TMaize/tmaize-blog)

# 介绍

一款 jekyll 主题，简洁纯净(主题资源请求<20KB)，未引入任何框架，秒开页面，支持自适应，支持全文检索

blog地址[qs Blog](https://qsblublu.github.io/qs.github.io/)

# 本地运行

jekyll 是使用 ruby 写的，所以先自行安装 ruby

```
# 第一次运行先执行 bundle install
bundle exec jekyll serve --watch --host=0.0.0.0 --port=8080
```

```
# 国内依赖下载慢可以使用ruby-china的镜像站进行请求重定向
bundle config mirror.https://rubygems.org https://gems.ruby-china.com
```

# 项目配置

1. 如果使用自己的域名，`CNAME`文件里的内容请换成你自己的域名，然后 CNAME 解析到`用户名.github.com`

2. 如果使用 GitHub 的的域名，请删除`CNAME`文件,然后把你的项目修改为`用户名.github.io`

3. 修改`pages/about.md`中关于我的内容

4. 修改`_config.yml`文件，具体作用请参考注释

5. 清空`post _posts`目录下所有文件，注意是清空，不是删除这两个目录

6. 网站的 logo 和 favicon 放在了`static/img/`下，替换即可，大小无所谓，图片比例最好是 1:1

7. 如果你是把项目 fork 过去的，想要删除我的提交记录可以先软重置到第一个提交，然后再提交一次，最后强制推送一次就行了

# 使用

文章放在`_posts`目录下，命名为`yyyy-MM-dd-xxxx-xxxx.md`，内容格式如下

```yaml
---
layout: mypost
title: 标题
categories: [分类1, 分类2]
---

文章内容，Markdown格式
```

文章资源放在`posts`目录，如文章文件名是`2019-05-01-theme-usage.md`，则该篇文章的资源需要放在`posts/2019/05/01`下,在文章使用时直接引用即可。当然了，写作的时候会提示资源不存在忽略即可

```md
![这是图片](xxx.png)

[xxx.zip 下载](xxx.zip)
```
