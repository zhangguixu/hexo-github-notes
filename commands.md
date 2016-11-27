# hexo命令

## 初始化项目

```shell
hexo init <folder>
```

会搭建项目的基础目录结构，并且安装好node依赖。

## 新建文章

```shell
hexo new [layout] <title>
```

新建一个文章，默认情况下会放置到/source/_posts目录下，且使用scaffolds中的post作为模板

可以通过`_config.yml`修改默认配置。

## 生成静态资源文件

```shell
hexo generate
```

可以添加两个option

|option|说明|
|:--|:--|
|-d|在生成静态文件之后进行部署|
|-w|监视源文件，实时编译|

## 发布

```shell
hexo public [layout] <filename>
```

## server

开启一个服务器，用于本地访问我们的博客

```shell
hexo server
```

可以添加以下option

|option|说明|
|:--|:--|
|-p, --port|指定一个端口|
|-s, --static|访问静态文件|
|-l, --log|开启日志|

## 部署

```shell
hexo deploy
```

部署博客

|option|说明|
|:--|:--|
|-g, --generate|先生成静态文件，然后再部署|

## 迁移

```shell
hexo migrate <type>
```

从其他的博客系统中迁移内容

## 清除

```shell
hexo clean
``` 

清理缓存文件db.json和public里的文件

