#C002-Eureka-Server
SpringCloud,Eureka-Server服务发现

# build
mvn clean package docker:build -DskipTests

# run
docker run -p 9999:9999 --name discover registry.cn-qingdao.aliyuncs.com/ac109/discover:1.6


## version
1.6
- 增加认证
1.5
- 更新SpringBoot 1.5.6,SpringCloud SR3 