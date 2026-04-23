---
name: help-me-write
description: "根据用户提供的参考材料撰写深度口播文案，支持科技、AI、软件等领域的视频脚本和文章创作，并自动发布到 GitHub 仓库。Use when the user shares reference materials and asks to write copy, draft a script, create an article, or produce content for video narration."
---

根据用户提供的材料，撰写一篇深度口播文案，输出为 Markdown 文件保存到项目根目录。

## 第一步：判断材料类型并学习风格

1. 如果材料涉及软件、AI、计算机等技术领域，先阅读 `references/` 目录下的所有范文，学习行文风格后再动笔。
2. 如果是其他领域的材料，无需参考范文，直接根据材料内容撰写。

## 第二步：撰写文案

按以下要求撰写：

- **结构**：正文分 2–4 个小节，每节用 `##` 标题。
- **节奏**：多用短句，逻辑清晰，段落过渡自然，适合口播朗读。
- **观点**：语气自信、果断，敢下结论，不模棱两可。
- **排除项**：不写画面调度或镜头指示。

输出文件命名格式：`项目根目录/<主题关键词>.md`

## 第三步：检查文案质量

发布前确认以下几点：

- 内容是否完整覆盖了参考材料的关键信息
- 行文风格是否与 `references/` 范文一致（仅限技术领域）
- 是否符合口播节奏要求（短句为主、过渡自然）

## 第四步：发布到 GitHub

1. 检查用户名下是否已有 `ai-docs` 仓库。
2. 如果没有，使用 `create_repository` MCP 工具创建该仓库。
3. 使用 `create_or_update_file` MCP 工具将文案上传到 `ai-docs` 仓库。
