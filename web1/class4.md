# Git Bash 常用命令
  
- git config --global user.name ""
- git config --global user.email ""  
设置用户名和邮箱，这里的用户名是 GitHub 的账号，邮箱是 GitHub 的绑定邮箱
- git clone https://github.com/username/仓库名 
克隆远程仓库到本地
- git status  
查看仓库中文件的状态
- git add file
- git commit -m "message"
- git push origin master  
以上三步为向远程仓库提交文档
- git config --global credential.helper store  
git push 免密