
## 搭建Spring-Framework环境
- Step1: Fork一下Spring官方Repository到自己的git Repository
- Step2: 拉取自己的git Repository中Spring-Framework项目, 然后用IDEA打开
- Step3: 配置Gradle设置, 1) use IDEA. 2) Gradle userHome. 3) 项目结构JDK版本
- Step4: 注释掉`./setting.gradle`文件中的 `id "io.spring.ge.conventions"`
- Step5: 刷新Gradle, 等待大约30分钟.


## Spring-Demo项目 - Spring日志 [mytest01](./spring01-mytest01)
- Step1: 创建Gradle项目.
- Step2: 测试各种日志框架. 结论: 普通项目中, 各种日志框架相互独立并不会产生冲突(但配置各是各的), 但Spring项目中日志框架会产生冲突(但配置文件是统一的)
- Step3: 使用JCL. 结论: JCL最大的问题是它不再维护了.
- Step4: 使用Slf4j. 结论: Slf4j官网提供了若干绑定器, 假如有新的日志工具出现,且官网没有提供绑定器, 也可以自己实现一个绑定器.
- 


## Spring-Demo项目 - 