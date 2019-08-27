# Dockerized Flowable

**flowable外接mysql数据库**

# Deployment
Start docker
```
docker run -p 8080:8080 wzhang2/flowable
```
Start docker with mysql
```
docker run -p 8080:8080 -e SPRING_DATASOURCE_DRIVER-CLASS-NAME=com.mysql.jdbc.Driver -e SPRING_DATASOURCE_URL=jdbc:mysql://ip:3306/flowable -e SPRING_DATASOURCE_USERNAME=mysql_user -e SPRING_DATASOURCE_PASSWORD=mysql_password wzhang2/flowable
```

##### 默认账号密码
user admin, password test

# 可选环境变量
```
SPRING_DATASOURCE_DRIVER-CLASS-NAME: f.e. com.mysql.jdbc.Driver  
SPRING_DATASOURCE_URL: f.e. jdbc:mysql://ip:3306/flowable  
SPRING_DATASOURCE_USERNAME: f.e. user_name  
SPRING_DATASOURCE_PASSWORD: f.e. password
```
# Repo
Download source
```
git clone https://github.com/zbaichuan1990/flowable.git
```
Generate flowable image
```
docker build -t wzhang2/flowable .
```
