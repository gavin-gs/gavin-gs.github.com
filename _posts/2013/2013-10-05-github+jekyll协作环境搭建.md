---

layout: post
title: 写作环境搭建(git+github+markdown+jekyll)
categories: 
- Programming
tags: 
- git
- github
- markdown
- jekyll

---

##参考文档
[写作环境搭建(git+github+markdown+jekyll)](http://site.douban.com/196781/widget/notes/12161495/note/264946576/)

##具体步骤如下：（以mac os为例）
1. 安装rubygems，macos默认安装，安装可以参考：[安装rubygems](http://hivelogic.com/articles/ruby-rails-leopard)
2. 安装相应的库，命令如下:	
	sudo gem install jekyll  
	sudo gem install directory_watcher
	sudo gem install liquid  
	sudo gem install open4  
	sudo gem install maruku  
	sudo gem install classifier  
	sudo gem install rdiscount

3. 在github上建立名为“username.github.com”(username为你的github的用户名)的项目
4. 打开终端，进入你的工作目录，然后将在第三步中建立的项目clone到本地，命令如下：git clone https://github.com/username/username.github.com username.github.com
5. 开始搭建博客，偷懒下载被人改好的jekyll框架，我用的是[kejinlu.github.com](https://github.com/kejinlu/kejinlu.github.com)，可以直接将这模版clone到本地，git clone https://github.com/kejinlu/kejinlu.github.com kejinlu，然后将内容拷贝到username.github.com目录中
6. 接下来就是修改刚才拷贝进来的内容，并做适当的修改，删除属于原来作者的所有东西，修改属于自己的，具体的修改可以参见我的源文件
7. 如果你的blog可以正确访问了，你就可以在_post目录下添加.md文件的博文了，命名规则为：yy-mm-dd-title.md(title就是你的博文的名字),写完之后上传到github上，就可以通过blog访问了
8. 如果你想现在本地查看一下博文的内容，在username.github.com目录下面，运行“jekyll serve”,运行成功后，在浏览器中访问：“localhost:4000”,就会看到你的blog显示出来了.
9. 注意事项：  
	1. 一定要删除“CNAME”文件  
	2. 先删除所有_post目录下的文件，这样就不会带上原作者的博文了  
	3. 修改每一处原作者的信息