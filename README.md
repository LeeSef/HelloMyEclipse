# HelloMyEclipse
Hello MyEclipse

//GitHub操作

1.问题：myEclipse无法pullGitHub
  解决方法：右击项目》》show in》》Git Repositories,找到config文件，修改为：
  [core]
	repositoryformatversion = 0
	filemode = false
	logallrefupdates = true
	[branch "master"] 
        remote = origin 
        merge = refs/heads/master 
  [remote "origin"] 
        url = https://github.com/LeeSef/HelloMyEclipse   
        fetch = +refs/heads/*:refs/remotes/origin/*
  注释：url为GitHub工程地址
  
