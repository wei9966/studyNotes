## Nginx实现反向代理

1. 创建两个tomcat挂载到docker容器下

2. 拉取nginx,然后进入nginx进行反向代理配置

3. ```
   docker inspect 容器名称 获取ip地址
   172.17.0.4 tomcat
   172.17.0.6 tomcat1
   ```