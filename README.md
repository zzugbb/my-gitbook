# my-gitbook

my-first-gitbook

<a href="https://travis-ci.org/zzugbb/my-gitbook" rel="nofollow">
  <img src="https://travis-ci.org/zzugbb/my-gitbook.svg?branch=master" alt="Build Status">
</a>

## gitbook项目初始化

```js
npm install gitbook -g //安装gitbook

//创建如下目录结构
my-gitbook/
├── README.md  //书籍介绍
└── SUMMARY.md //书籍目录结构

gitbook init //创建 SUMMARY.md 中的目录结构
gitbook serve //编译 && 预览

gitbook build // 编译-生成 _book/
```

## 本项目使用

```js
1. git clone https://github.com/zzugbb/my-gitbook.git
2. 修改书籍文件，md文件.(master分支)
3. 提交代码到远程.(master分支)
4. 触发自动构建.
```

## 部署说明

* master: 保存书籍的源码
* gh-pages: 发布后的静态页面，即 _book/ 下面内容，便于页面访问

## 参考

* [gitbook教程](http://www.chengweiyang.cn/gitbook/introduction/README.html)