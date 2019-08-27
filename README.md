# Dockerized Flowable

**flowable外接mysql数据库**

# Deployment
Download source
```
git clone https://github.com/zbaichuan1990/flowable.git
```
Generate flowable image
```
docker build -t wzhang2/flowable .
```
Start docker
```
docker run -p 8080:8080 wzhang2/flowable
```
##### 默认账号密码
user admin, password test

# 可选环境变量
*SPRING_DATASOURCE_DRIVER-CLASS-NAME: f.e. com.mysql.jdbc.Driver*

*SPRING_DATASOURCE_URL: f.e. jdbc:mysql://ip:3306/flowable*

*SPRING_DATASOURCE_USERNAME: f.e. user_name*

*SPRING_DATASOURCE_PASSWORD: f.e. password*
