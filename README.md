# pi-agent-practice

- **个人实验报告**：`report/README.md`
- **仓库地址**：[https://github.com/3478415652/pi-agent-practice](https://github.com/3478415652/pi-agent-practice)

## 项目简介

本仓库是「实践课1：Pi Agent 安装与使用」的个人作业。Pi 是命令行 AI 编码客户端，本次安装的是客户端本身，不涉及大模型权重部署，也不编译上游仓库。

任务链条：本地安装并启动 → 配置模型跑通一次会话 → 切换模型与思考级别 → @ 引用代码文件、粘贴小图片 → 从 Pi Packages 选装插件并实测 → 让 AI 安装 pptx Skill 并调用。

## 目录结构

```text
pi-agent-practice/
├── report/             # 个人实验报告与截图
│   ├── README.md       # 报告正文（逐项过程 + 截图说明 + 问题处理 + 原理理解）
│   └── images/         # 13 张关键截图
├── pi-test/            # 任务四的练习目录
│   └── hello.py        # add(a, b) 示例，供 @ 引用
├── .pi/
│   └── skills/
│       └── pptx/       # 选做任务安装的 PPT Skill（SKILL.md / LICENSE.txt / scripts）
└── README.md           # 本文件，仓库总览
```

`report/` 是人工维护的内容，`.pi/skills/pptx/` 由任务六中 Pi 自行下载安装（58 个文件，附 `SOURCE.json` 记录源 commit）。

## 常用命令

```powershell
# 启动（在项目目录内启动才会加载 .pi 下的 Skill）
cd D:\project\git\pi-agent-practice
pi

# 查看已安装的插件及来源
pi list
```

> 本机 Pi 托管安装在 `D:\APP\PiAgent`，通过用户环境变量 `PI_CODING_AGENT_DIR` 与新 PATH 首项生效。