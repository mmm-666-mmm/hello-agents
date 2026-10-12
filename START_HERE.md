# Hello-Agents 学习子项目

本项目用于边做边学，目标是为 Agent 算法实习打基础。

## 来源

- 上游：https://github.com/datawhalechina/hello-agents
- 获取日期：2026-10-12（北京时间）
- 来源版本：main 分支源码压缩包；未包含 Git 历史。
- 上游教程、示例与许可证保留在原目录。

## 目录入口

- `README.md`：上游教程总目录。
- `docs/`：各章中文正文及图片。
- `code/`：上游配套代码。
- `learning/notes/`：自己的学习笔记。
- `learning/exercises/`：自己编写或修改的练习。
- `learning/experiments/`：对照实验及结果记录。

## 第一次从这里开始

1. 阅读 `docs/chapter1/第一章 初识智能体.md`，理解模型、工具、环境和行动循环。
2. 阅读 `docs/chapter3/第三章 大语言模型基础.md`，遇到陌生概念先记录下来。
3. 阅读 `docs/chapter4/第四章 智能体经典范式构建.md`，对照 `code/chapter4/ReAct.py` 追踪执行过程。
4. 在 `learning/notes/01-first-agent.md` 中记录模型输入、工具调用、工具结果和终止条件。

Python 按代码需要补：先学列表、字典、函数、类、模块导入和异常处理。暂时不需要把整个语言学完。

## 当前环境状态

源码已下载。尚未创建 Python 虚拟环境、安装依赖、配置模型服务或运行示例。
运行第一个模型示例前，需要选择模型服务并配置对应环境变量；也可以后续配置本地模型。
RTX 4060 的具体显存尚未确认，模型训练配置留到训练阶段确定。

## 算法学习的验收方式

先跑通一个最小 Agent，再比较不同决策策略。记录任务成功率、模型调用次数、耗时与失败原因。
进入第十一章 Agentic-RL 前，补齐 PyTorch、SFT 和强化学习基础。
