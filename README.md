# wings-frame-dev
Open-Source Framework For Wings (Hangzhou) Software Technology Co., Ltd.

# wings-frame

### project structure
* spring-boot-starter-parent
* spring-boot-starter-data-redis
* mybatis-spring
* spring-api
* spring-boot-starter-aop
* spring-boot-starter-mail
* spring session security or shiro
* spring-boot-starter-web


### Open-Source Framework For [Wings](https://www.wings90.com)
       
*  [https://github.com/vivioning/wings-frame](https://github.com/vivioning/wings-frame)

*  [ Wings (Hangzhou) Software Technology Co., Ltd.](https://www.wings90.com)

### Mail list

* [wings60@163.com](wings60@163.com)

* QQ: waiting 
---
## Quick start 

```xml
        <dependency>
            <groupId>com.wings</groupId>
            <artifactId>wings-frame-database</artifactId>
            <version>1.0-SNAPSHOT</version>
        </dependency>
        
        <dependency>
            <groupId>com.wings</groupId>
            <artifactId>wings-frame-bootstrap</artifactId>
            <version>1.0-SNAPSHOT</version>
        </dependency>
```


### configuration file processing
* redis config
```properties
    redis.maxTotal=1024
    redis.maxIdle=200
    redis.maxWaitMillis=1000
    redis.host=10.0.0.30
    redis.port=6379
    redis.timeout=15000
    redis.password=123456
```

* database config
```properties
    mybatis.url=jdbc:mysql://10.0.0.30:3306/essay?useUnicode=true&characterEncoding=UTF-8&useSSL=false&serverTimezone=GMT%2B8&zeroDateTimeBehavior=convertToNull
    mybatis.driverClassName=com.mysql.jdbc.Driver
    mybatis.username=root
    mybatis.password=123456
    mybatis.defaultAutoCommit=false
    mybatis.initialSize=30
    mybatis.maxActive=150
    mybatis.minIdle=5
    mybatis.maxIdle=20
    mybatis.maxWait=3000
    mybatis.logAbandoned=true
    mybatis.removeAbandoned=true
    mybatis.removeAbandonedTimeout=180
    mybatis.testWhileIdle=true
    mybatis.testOnBorrow=false
    mybatis.testOnReturn=false
    mybatis.validationQuery=select 1
    mybatis.timeBetweenEvictionRunsMillis=30000
    mybatis.minEvictableIdleTimeMillis=10000
    mybatis.numTestsPerEvictionRun=100
```
* mybatis config
```properties
    mybatis.typeAliasesPackage=com.wings.xxx.bean
    mybatis.mapperLocations=classpath:mappers/*.xml
    mybatis.config-location=classpath:mybatis-config.xml
    mybatis.basePackage=com.wings.xxx.dao
```
