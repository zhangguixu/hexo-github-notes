# 安装主题

[NexT主题](http://theme-next.iissnan.com/)

## 1. 下载

下载到hexo项目目录下

```shell
cd hexo-demo
git clone https://github.com/iissnan/hexo-theme-next themes/next
```

## 启用主题

编辑`_config.yml`，找到`theme`，将其值改为`next`

先运行`hexo clean`，清理缓存，之后再验证切换主题之后的效果

```shell
hexo clean
hexo generate
hexo server -s
```

## 主题样式设定

通过`/themes/next/_config.yml`中的`scheme`来设置不同的样式。

* Muse : 默认，黑白主调，大量留白
* Mist : 整洁有序的单栏外观(选用)
* Pisces : 双栏外观

## 设置语言

同样是`_config.yml`，设置`language`为`zh-Hans`

## 设置头像

在`/themes/next/_config.yml`找到`avatar`，根据提示，将其值设为`/uploads/avatar.jpg`（其他格式的也行，后缀对得上即可），我们在source下创建一个新的目录`uploads`，然后将我们的头像放置上去，重新生成静态资源即可。

## 设置社交信息

在`/themes/next/_config.yml`找到`social_icons`,设置链接