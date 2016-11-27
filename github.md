# 配置github

在本地已经弄好了hexo项目，配置好主题之后，我们来看看如何用github来关联和部署我们的静态页面。

## 1. 新建repository

新建一个github的repository，将其命名为`your_user_name.github.io`（固定写法）

## 2. 配置本地`_config.yml`

```yml
deploy:
    type : git
    repo : https://github.com/zhangguixu/zhangguixu.github.io.git
    branch: master
```

然后执行

```shell
npm install hexo-deployer-git --save
```

## 3. 部署页面

执行部署，部署的步骤可以为

```shell
hexo clean
hexo generate
hexo deploy
```

然后在浏览器中输入`http://zhangguixu.github.io/`就可以看到效果
