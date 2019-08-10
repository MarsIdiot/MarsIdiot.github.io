# MarsIdiot.github.io
***MarsIdiot's  first  blog***

## 1、本地开发

####环境及启动

1.检查是否已安装 Ruby 2.1.0 或更高版本
    $ ruby --version
    > ruby 2.X.X

 【注意】安装时一定要选择 utf-8编码  否则后面安装'gem install bundler' 等会出现编码错误,导致安装失败。

2. 安装 Bundler：

$ gem install bundler

项目配置启动，在需要开发的根目录

 3.安装 Jekyll 和其他依赖项 

 bundle install

若出现bundle install 长时间无响应？原因有两个，如下：

原因一：great wall fire的原因，国外资源无法访问，需修改gem的source
	1）gem sources --remove https://rubygems.org/
	2）gem sources -a https://gems.ruby-china.com/
	3）安装好后用gem sources -l 检查当前SOURCES列表

原因二：Gem的source设置不正确
在Gemfile中source需要改为刚换的资源镜像服务器  source 'https://gems.ruby-china.com/'

4. 本地Jekyll站点服务启动
    bundle exec jekyll serve

5.预览本地 Jekyll 站点，网址为：http://localhost:4000
