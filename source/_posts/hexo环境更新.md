---
title: hexo环境同步
date: 2017-03-05 15:42:00
tags:
---
当我们在第二台电脑想继续更新自己博客。
步骤一：电脑一：新建分支并push：
	git branch hexoblog
	git add .
	git commit -m "hexo环境"
	git push -u origin hexoblog
步骤二：电脑二：clone到本地
	git clone https://github.com/youngda/youngda.github.io.git
	下载安转hexo
	sudo npm install -g hexo-cli
	安装:ps(seve前面两个横线，这是排版问题吗...)
	sudo npm install hexo-deployer-git --save
	sudo npm install
步骤三：工作就完成了，开始新建博客吧！
	hexo new "hexo环境同步"
	生成静态页面:	
	hexo generate
	将文章部署到Github:
	hexo deploy
步骤四：如果你需要来回切换电脑的话，别忘了	
	git push -u origin hexoblog
