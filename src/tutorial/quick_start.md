## 快捷创建智能体

cota提供了不同场景的智能体示例，方便用户测试和参考，可以通过执行以下命令获取

```bash
cota init
```

初始化后会得到如下目录
```
bots/
├── agent.yml
├── endpoints.yml
├── actions/
│   ├── Query.yml
│   ├── Response.yml
│   ├── Selector.yml
│   ├── Calculate.yml
│   └── Weather.yml
└── dialogue.yml
```


agent.yml
该文件定义了机器人的行为和对话流程。关键配置项包括：

actions: 定义了机器人可以执行的动作。
dialogue: 定义了对话的模式和限制。
endpoints.yml
该文件定义了机器人的后端服务和LLM（语言模型）的连接信息。关键配置项包括：

base_store: 数据库连接信息。
channel: 消息通道（如Redis）的连接信息。
llm: 语言模型的连接信息，包括模型类型、API类型、API密钥和API基础URL。



## 运行智能体
```bash
cota shell
```



