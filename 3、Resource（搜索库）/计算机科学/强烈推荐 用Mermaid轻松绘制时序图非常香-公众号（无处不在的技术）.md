https://mp.weixin.qq.com/s/fU_csbFq25eALULaOyALMQ
## **什么是Mermaid**

Mermaid是一个开源的图表库，它允许我们使用简单的文本语法来定义和绘制各种类型的图表，包括流程图、时序图、甘特图等。Mermaid支持多种输出格式，包括SVG、PNG和PDF，使得生成和共享图表变得非常方便。

官方地址为：https://mermaid.js.org/

官方的在线编辑效果预览地址为：https://develop.git.mermaid.live/edit

官方的关于[[时序图]]的说明文档：http://mermaid.js.org/syntax/sequenceDiagram.html

```
sequenceDiagram    
    participant User    
    participant Application    
    participant SpringBoot    
    participant DataSource    
    participant Service
    
    User->>Application: 打开应用程序    
    Application->>SpringBoot: 启动Spring Boot应用    
    SpringBoot->>DataSource: 初始化数据源    
    DataSource-->>SpringBoot: 返回数据源配置    
    SpringBoot->>Service: 注册服务    
    Service-->>SpringBoot: 返回服务注册结果    
    SpringBoot-->>Application: Spring Boot启动成功    
    Application-->>User: 显示应用界面
```