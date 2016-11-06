##Gradle SpringMVC Mybatis构建web应用

###框架组成

- Gradle > [init project](https://github.com/silence940109/Java/tree/master/Gradle_STS_Create) > finished > 2016-10-23
- Gretty > Server hot deploy > [tomcat热部署方案](https://github.com/silence940109/Java/tree/master/Gradle_Gretty) > finished > 2016-11-05
- Spring 4.25 > finished > 2016-10-23
- Scala 2.1
- Spark 2.0.0
- SpringMVC4.25 > finished > 2016-10-25
- MyBatis3.3.0
- Freemarker
- Druid数据库连接池(连接池监控) > [Spring Druid](https://github.com/silence940109/Java/tree/master/Alibaba_Druid) > finished > 2016-10-26
- Quartz2.1作业调度 > finished > 2016-10-27
- Lucene6.2.1全文信息检索
- Redis
- Redis客户端开发包Jedis
- Ehcache
- sf4j日志->log4j日志引擎 > finished > 2016-10-20
- JUNIT单元测试
- Strman-java字符处理
- Tablesaw-伪“大数据”处理
- Dex-数据可视化
- Swagger > API文档 > RESTFUL API TEST > finished 2016-11-03
- Fastjson > JSON处理器
- Mysql

###要求

- Gradle 3.1
- JDK 1.7+
- Scala 2.1+
- Tomcat7+(关于gradle使用tomcat插件，你可以在[Gradle Tomcat plugin](https://plugins.gradle.org/plugin/com.bmuschko.tomcat))查看
- MySQL5.5+

###配置

- 在src/main/resources/db.properties配置数据库信息
- 在src/main/resources/spring-quartz-task.xml配置作业调度信息 

###运行

- git clone https://github.com/silence940109/SSM.git

- cd SSM 

- gradle appRun

- 访问http://localhost:8080/SSM 

###详情

####关于Gretty插件配置热部署方案，请看[这里](https://github.com/silence940109/Java/blob/master/Gradle_Gretty)

![](https://github.com/silence940109/Java/blob/master/Gradle_Gretty/image/1.png)

####关于Alibaba Druid数据源监控配置
关于Alibaba Druid数据源监控配置的信息详情，可以看

在web.xml中配置druid入口的用户名和密码

[Alibaba Druid数据源监控配置](https://github.com/silence940109/Java/tree/master/Alibaba_Druid)这里

运行结果

![](https://github.com/silence940109/Java/blob/master/Alibaba_Druid/1.png)

![](https://github.com/silence940109/Java/blob/master/Alibaba_Druid/2.png)

####关于Swagger UI API测试
系统已经集成了swagger，关于spring如何集成和配置swagger，请看[这里](https://github.com/silence940109/Java/tree/master/swagger)

服务器运行起来后，你可以在浏览器中打开`http://localhost:8080/SSM/swagger/index.html`

在输入框输入`http://localhost:8080/SSM/api-docs`,然后就可以看到以下的界面，你可以很方便的进行测试

![](https://github.com/silence940109/Java/blob/master/swagger/image/index.png)