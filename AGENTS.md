# Agents.md — AI 操作指南

> 本文件是给 AI（Claude、Codex 等）阅读的知识库操作手册。
> 在对知识库进行任何读写操作前，请先阅读本文件。

## 1、目录说明

1. 这个目录`.ai-context`，存放与AI所有的上下文，AI 需要以这个目录下的文档作为第一参考。
2. `.ai-context/SOP` 目录存放标准行为文档，当我指定使用某个行为文档时，再去读取响应文档，平时不需要访问和读取该 SOP 目录下文档。
3. `.ai-context/CONTENT`目录下，存放我与AI交谈的历史任务，文件名会按照数字编号命名。这个目录下的每个文件头部，都有状态信息`STATUS`，如果状态标记为`archived`或`已归档`，则无需再阅读文档后面的内容，除非我在命令中强制指定阅读。
4. `.ai-context/TEMPLATE`下是一些模版文件。每个模版包含空的模板[template_name.md]和一个实例模板[template_name.example.md].这个目录下的模板文件，如果我没有主动提到去阅读它，不要去读取或者更改他们的内容。

## 2、特定行为

1. 任务执行完成或者任务需要人工审批时，在终端调用"m-notify bark <content> --title <title>",title 固定为"Codex",<content>则是相应内容。这样，会通过bark发消息到我的手机上。
