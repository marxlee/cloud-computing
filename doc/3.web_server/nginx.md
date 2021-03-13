# Nginx服务器配置
下载地址：
http://nginx.org/en/download.html

#
1.在nginx安装包下，双击nginx.exe启动nginx服务器<br/>

2.或者选择在cmd黑窗口进入此包输入nginx启动服务器（推荐）<br/>
浏览器输入：localhost:80查看Nginx欢迎页面标识启动成功<br/>

3.配置nginx配置文件，conf/nginx.conf<br/>
```
    #新增配置windows系统配置
    server{
         listen       9901; 
         server_name	localhost;
  		location / { 
     	 root   D:\workspace_image_server; # windows路径
    	 index  index.html index.htm;
  		}
  	}
```

4.重启nginx服务器，保存一张图片输入目标地址 http://localhost:9901/test01.jpg 查看是否访问成功。<br/>

