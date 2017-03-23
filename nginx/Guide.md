# nginx documentation  
该文件为nginx学习笔记,主要参考官网document。
=================================================

## Beginner's Guide   
nginx有一个主进程和多个工作进程，主进程负责读和评估配置文件，维护工作进程；工作进程负责处理实际的请求。

### Starting,Stoping,and Reloading Configuration   
nginx -s singal  
* stop  立刻停止  
* quit  等待工作进程结束后停止  
* reload  重载配置文件  
* reopen  重新打开日志文件  
