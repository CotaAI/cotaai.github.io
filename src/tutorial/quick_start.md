## 快捷创建智能体

cota提供了不同场景的智能体示例，方便用户测试和参考，可以通过执行以下命令获取

```bash
cota init
```

执行上面初始化命令后，得到cota_projects目录
```
cota_projects
├── simplebot
│   ├── agent.yml
│   └── endpoints.yml
└── taskbot
    ├── agent.yml
    ├── endpoints.yml
    └── task.yml
```
simplebot 和 taskbot是两个agent实例，分别代表了简单的问答agent和任务执行agent。

## 文件释义
agent.yml 定义了智能体的结构和基本要素。
endpoints.yml 定义运行服务的基本要素，如数据库链接、通信使用的通道配置、LLM token配置等。

## 运行智能体
可以选着cota_projects中的任一个智能体运行。在运行之前，需要修改endpoints.yml文件，补全基本的配置；如LLM的token等。

命令行体验agent，进行交互
```bash
cota shell
```

也可以将cota部署成服务
```bash
cota run
```



