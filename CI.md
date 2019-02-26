# 持续集成

## 什么是持续集成？

> 持续集成（英语：Continuous integration，缩写 CI）是一种软件工程流程，是将所有软件工程师对于软件的工作副本持续集成到共享主线（mainline）的一种举措。

本次我们以 `gitbook` 为例，只要修改了书籍源文件，提交代码到远程，自动触发构建，生成静态页面提供访问。

## 注册 Travis CI 账号，绑定 GitHub 账户

首先，我们到 [Travis CI 官网](https://travis-ci.org/) 用自己的 GitHub 账户直接关联登录，并允许 Travis CI 查看自己的公有仓库。

然后我们到 [Travis CI 账户页面](https://travis-ci.org/account/repositories), 开启对应工程, 如下：

<img src="img/shili1.jpg">

## 配置持续集成文件

`.travis.yml` 是 `Travis CI` 的部署配置文件，`Travis CI` 部署时会自动读取我们每次 Commit 中是否包含 .travis.yml，有此文件才会开始部署。

### 创建 `.travis.yml` 配置文件