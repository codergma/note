# nginx documentation  </br>
该文件为nginx学习笔记,主要参考官网document。
=================================================

## Beginner's Guide   
nginx有一个主进程和多个工作进程，主进程负责读和评估配置文件，维护工作进程；工作进程负责处理实际的请求。
配置文件位置：/usr/local/nginx/conf, /etc/nginx, or /usr/local/etc/nginx   

### Starting,Stoping,and Reloading Configuration   
nginx -s singal  
* stop    立刻停止  
* quit    等待工作进程结束后停止  
* reload  重载配置文件  
* reopen  重新打开日志文件  
* nginx -c /etc/nginx/nginx.conf 启动


### Configuration File’s Structure
简单指令:空格分割，分号结尾。  
块指令：大括号包裹。  
> 没有上下文的指令，上下文默认是main;  
> events,http 上下文是main;  
> server上下文是http;  
> local 上下文是server;    


### Setting Up a Simple Proxy Server  
指令：proxy_pass  


### Setting Up FastCGI Proxying



