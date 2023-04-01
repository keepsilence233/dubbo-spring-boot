# Apache Dubbo Spring Boot Project

# 使用Nacos作为注册中心

Nacos安装方式：https://github.com/nacos-group/nacos-docker/blob/master/README_ZH.md

如果机器为m1的mac,可以使用该镜像：https://github.com/alibaba/nacos/issues/6340

启动成功后访问：http://localhost:8848/nacos/#/login  默认用户名密码：nacos/nacos



# 示例项目说明

## 版本对应关系

https://github.com/apache/dubbo-spring-boot-project/blob/master/README_CN.md

### dubbo version

```xml
<!-- https://mvnrepository.com/artifact/org.apache.dubbo/dubbo-spring-boot-starter -->
<dependency>
    <groupId>org.apache.dubbo</groupId>
    <artifactId>dubbo-spring-boot-starter</artifactId>
    <version>3.0.7</version>
</dependency>
```

### SpringBoot version

```xml
    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>2.3.1.RELEASE</version>
        <relativePath/> <!-- lookup parent from repository -->
    </parent>
```

### Dubbo Nacos Register version

```xml
<!-- https://mvnrepository.com/artifact/org.apache.dubbo/dubbo-registry-nacos -->
<dependency>
    <groupId>org.apache.dubbo</groupId>
    <artifactId>dubbo-registry-nacos</artifactId>
    <version>3.0.7</version>
</dependency>
```



## 项目模块

### order-service(订单服务)

- 子模块：order-api ：定义服务接口

- 子模块：order-controller：服务提供端

  app service、 domain service、repository 层忽略

### oms(订单管理服务)

- 子模块：oms-api：对外服务接口
- 子模块：oms-controller：请求order-service服务接口,返回结果





