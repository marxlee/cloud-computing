# Git 常见问题
### 命令行常出现输入用户名密码
git config --global credential.helper store

### ERROR:remote: HTTP Basic: Access denied
fatal: Authentication failed for 'http://****.git/'  
Resolve:  
git config --system --unset credential.helper  

