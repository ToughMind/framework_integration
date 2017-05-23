# springboot1.5.3+mybatis3.4.4整合

## 项目框架结构图


## 简要说明

1、 集成了swagger2（包括其ui界面），可以撰写api文档

2、 

## 疑难点
### spring boot应用入口
- 官方建议，入口类不要写在默认目录下（理论上实战开发中不会这么设计）。

- 入口类放在根包路径下，那么可以使用`@SpringBootApplication`来代替三个注解`@Configuration``@EnableAutoConfiguration``@ComponentScan`

- 入口类继承SpringBootServletInitializer并重写configure方法。运行主方法后，会将我们的web项目打包成war，并默认启动一个端口为8080的tomcat容器来运行我们的Web项目。