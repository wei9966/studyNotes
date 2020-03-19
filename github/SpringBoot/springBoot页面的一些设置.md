如何设置springBoot的一些设置
-------------------
1. 1 在mvcConfig类上添加@configuration注解
2. 2 继承WebMvcConfigurationSupport
2. 3 配置初始进入页面
    1. 3.1 重写 addViewControllers(ViewControllerRegister register)方法
    2. 3.2 调用register的addViewController("url").setViewName("网页前缀名");
    3. 3.3 调用register的setOrder(Ordered.HIGHEST_PRECEDENCE);
    4. 3.4 在super.addViewControllers()
3. 4 配置静态资源路径
    1. 4.1 重写 addResourceHandlers(ResourceHandlerRegister register)
    2. 4.2 调用register的addResourceHandler("/static/**").addResourceLocations(ResourceUtil.CLASSPATH_URL_PREFIX+"/static/");
    3. 4.3 super.addResourceHandlers()
4. 5.解决controller返回字符串中文乱码
    1. 5.1 重写extendMessageConverters(List<HttpMessageConverters<?>> converters)
    2. 5.2 for循环遍历converters
    3. 5.3 判断 converter instanceof StringHttpMessageConverter
    4. 5.4 强转convertes为StringHttMessageConverter并调用setDefaultCharset(StandardCharsets.UTF-8);