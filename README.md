# guangheApps.github.io

## 使用教程
[Hexo 官方教程](https://hexo.bootcss.com/docs/writing.html)

[Wikitten主题教程](https://github.com/zthxxx/hexo-theme-Wikitten/blob/master/README_zh-CN.md)

[使用Hexo框架搭建博客，并部署到github上](https://segmentfault.com/a/1190000018250408)

## 同步到本地

### 本机安装hexo

全局执行

`npm install -g hexo-cli`

### 将站点仓库拉到本地

> 注意：本仓库是部署仓库，不是站点仓库，站点仓库里的才是网站原始配置

`git clone git@github.com:guangheApps/website.git`

### 初始化hexo服务

> 因为已经拥有了hexo配置环境，所以无需初始化hexo了，初始化服务即可

`npm install hexo-server --save`

`hexo clean`

`hexo g`

`hexo s`

本地查看本地local:4000端口在浏览器是否可以正常展示网页即可，如果可以打开，本地环境就配置完成了，如果打开网站空白，查看命令行输出是否为`layout no index`之类的提示，如果是，说明主题包没能成功拉下来

进入站点仓库的 `/themes` 文件夹，手动删除 `Wikitten` 文件夹

然后按照 [Wikitten主题教程](https://github.com/zthxxx/hexo-theme-Wikitten/blob/master/README_zh-CN.md) 操作一遍，再执行一遍


`hexo clean`

`hexo g`

`hexo s`

此时应该可以显示内容了
