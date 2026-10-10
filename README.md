# EyeCare

EyeCare 是用于 Craft Agents 工作区的眼科就诊准备场景 Skill。当前版本演示如何让 Agent 在回答预约前准备问题时核对资料来源、区分行政信息与医疗问题，并在信息不足时明确停止。

## 当前范围

- 提供可安装的工作区 Skill 和合成演示资料。
- 可以回答演示资料中明确写出的就诊准备与预约核对问题。
- 不包含医院 API、患者系统连接器、真实预约查询、诊断建议或自动办理业务的能力。

## 安装与演示

1. 安装 [Craft Agents](https://github.com/craft-ai-agents/craft-agents-oss)，在应用中创建一个工作区。
2. 将本仓库的 `skills/eyecare-visit-prep/` 复制到该工作区的 `skills/` 目录下。Craft Agents 的工作区配置通常位于 `~/.craft-agent/workspaces/{id}/`。
3. 在该工作区的对话中提及 `eyecare-visit-prep`，例如：`请使用 eyecare-visit-prep，告诉我预约前需要核对什么。`
4. 用 [演示问题](examples/demo-questions.md)检查资料缺失、真实预约查询和医疗问题的处理方式。

Skill 只读取仓库内的合成资料。要服务真实机构，需要另行接入授权数据源、权限校验、人工接管和评测；本仓库未提供这些实现。

## 项目来源

本仓库只发布 EyeCare 场景文件，不复制 Craft Agents 应用源码。Craft Agents 由 Craft Docs Ltd. 开发，原项目采用 Apache 2.0 许可证；本项目与其官方团队没有隶属或背书关系。详见[原项目](https://github.com/craft-ai-agents/craft-agents-oss)及其许可证和商标说明。
