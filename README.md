个人博客模板
================
基于Jekyll+Github构建，支持PC与智能机访问。   
特有功能：支持按栏目及标签的列表显示，栏目可分页显示。  
演示地址：[https://panxw.github.com](http://panxw.github.com)  
项目代码：[项目代码](https://github.com/panxw/panxw.github.com)  

## 1.环境准备
由于用到自定义插件(Gitpage不支持)，本地必须有运行环境支持。  
1.安装ruby运行环境(请自行搜索安装方法)。  
2.安装bundler(gem install bundler)。  

## 2.博客项目准备
1.注册一个Github账号。  
2.新建博客项目，项目名称：username.github.io (username为github账号名)   
3.将该博客项目克隆至本地。  

## 3.使用本博客模板操作步骤
1,下载本项目代码，解压后放入博客项目根目录，然后cmd进入，执行bundle install。  
2,修改_config.yaml及about.md文件，以配置站点、栏目及个人信息。  
3,修改_include目录下相关文件，以配置网站统计(analytics.html)，网友评论(comment.html)，右侧栏目(categories.html)等。  
4,修改CNAME及robots.txt文件，以绑定自己的域名。  
5,删除_posts目录下所有文件，添加自己的栏目及文章。  
6,执行bundler exec jekyll serve  -d docs启动服务。  
7.查看运行效果: http://localhost:4000  
8.git add .  
9.git commit -m "update content"  
10.正常流程提交代码到Github。  
11.项目主页->Settings->GitHub Pages->"Check it out here!"->Source，选择master分支，docs目录。  
12.查看博客，地址：https://username.github.io  
*注：提交代码后要等待几分钟生效*    


## 4.本博客模板使用了
1,CNZZ的网站统计服务，官网：http://cnzz.com  
2,来必力的网友评论服务，官网：https://www.livere.com  
3,Google 的Adsense广告，官网：https://www.google.com/adsense/login/zh_CN  
如需查看或管理网站统计、评论或广告，请自行注册帐号，然后修改_includes目录下相关文件。  

## 5.联系交流
邮箱：email(winfirm#qq.com)  

## License
    Apache 2.0
