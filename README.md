# Spingboot 学习
 - maven创建项目
 - 日志使用 Slf4j + logback (springboot默认)
    - 配置文件
    - 更改日志框架
 - 全局异常
    - 处理参数确实异常
    - 处理空指针异常
    - 自定义异常
 - 切面AOP
    - 切点 `@Pointcut`
    - 执行前 `@Before`
    - 执行后 `@After`
    - `@AfterReturning` 注解和 `@After` 有些类似，区别在于 `@AfterReturning` 注解可以用来捕获切入方法执行完之后的返回值
    - `@AfterThrowing` 注解是当被切方法执行时抛出异常时，会进入 `@AfterThrowing` 注解的方法中执行，在该方法中可以做一些异常的处理逻辑
 - myBatis
    - 基于注解的整合
    - 基于xml的整合
 - 监听器
    - 监听servlet上下文：初始化数据
    - 监听session：获取在线人数
    - 监听servlet request
    - 自定义监听
 - 拦截器
    - 自定义拦截器对象，包含`preHandle()` `postHandle()` `afterCompletion()`
    - 拦截器配置，spring boot 2.0之前继承`WebMvcConfigurerAdapter`类,2.0之后继承`WebMvcConfigurationSupport`类
    - 会产生静态资源被拦截的问题，重写`addResourceHandlers`方法
 - Redis
    - 引入Redis依赖
    - 配置Redis
    - 使用StringRedisTemplate对Redis进行操作
 - Thymeleaf模板引擎
    - 错误页面自动配置 /templates/error 4xx.html 5xx.html
    - 对象、数组的使用  
 - ActiveMq消息队列
    - 配置连接url: tcp://localhost:61616 
    - 管理 http:localhost:8161/admin 用户名和密码为admin
    - 目的地（Queue Topic）
    - 发送者
    - 消费者
    - 点对点模式（Queue） 发布/订阅模式（Topic）
 - 权限管理（Shiro）
    - 三大组件 `Subject`、`SecurityManager` 和 `Realm`
    - 权限认证 `权限`，`角色`和`用户`
    - spring security
 - 邮件
    - 生成授权码
    - 引入依赖，配置spring.mail
    - 利用JavaMailSender配置MailService
    - 测试
    