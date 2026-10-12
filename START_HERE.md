# Hello-Agents 学习子项目

本项目用于边做边学，目标是为 Agent 算法实习打基础。

## 来源

- 上游：https://github.com/datawhalechina/hello-agents
- 获取日期：2026-10-12（北京时间）
- 来源版本：从个人 Fork 的 main 分支通过 Git 克隆，保留完整提交历史。
- 个人仓库：https://github.com/mmm-666-mmm/hello-agents
- Git 远程：origin 指向个人仓库；upstream 指向上游教程仓库。
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

已独立安装 Python 3.13.16（64 位），位置为 `C:\Program Files\Python313`。
项目虚拟环境位于 `.venv/`，已安装并验证 `requests`、`tavily-python`、`openai`，不依赖 Codex 自带 Python。
尚未配置模型服务或运行联网模型示例。
运行第一个模型示例前，需要选择模型服务并配置对应环境变量；也可以后续配置本地模型。
RTX 4060 的具体显存尚未确认，模型训练配置留到训练阶段确定。

### 在 PowerShell 中使用

安装 Python 后，关闭旧终端并新开一个 PowerShell，以加载更新后的 PATH。

```powershell
cd C:\Users\Administrator\Desktop\m\hello-agents
python --version
.\.venv\Scripts\python.exe --version
# 运行自己的脚本：
# .\.venv\Scripts\python.exe learning\exercises\你的脚本.py
```

上述方式无需激活环境。给项目安装依赖时使用 `.\.venv\Scripts\python.exe -m pip`。
如果需要重建环境：

```powershell
py -3.13 -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r learning\requirements-first-agent.txt
```

如果 PyPI 连接失败，可以在安装命令末尾加上 `--proxy http://127.0.0.1:7897`，前提是本机代理正在该端口运行。
`.venv/` 已由 Git 忽略，不上传到 GitHub。

## 算法学习的验收方式

先跑通一个最小 Agent，再比较不同决策策略。记录任务成功率、模型调用次数、耗时与失败原因。
进入第十一章 Agentic-RL 前，补齐 PyTorch、SFT 和强化学习基础。
