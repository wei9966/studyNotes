SpringBoot核心注解
--------------
- 1.@SpringBootApplication:代表springBoot的启动类

- 2.@SpringBootConfiguration:通过bean对象来获取配置信息.被@Configuration所注解

- 3.@Configuration:通过对bean对象的操作替代Spring中的XML文件

- 4.@EnableAutoConfiguration:完成一些初始化环境的配置.

- 5.ComponentScan:来完成spring的组件扫描,替代之前我们在xml文件中配置组件扫描的配置

  ```
  <context component-scan pacage="">
  ```

- 6.@RestControoler:由@Controller和@ResonseBody 注释的controller中的方法会以json格式返回数据