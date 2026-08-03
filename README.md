# Seedance 2.5 Script to Prompt Skill

Simply provide a script or describe your idea in natural language, and this skill will generate prompts in a standardized format optimized for Seedance 2.5. It is based on the official Seedance 2.5 user guide.

> This is an unofficial community project and is not affiliated with or endorsed by Jimeng or ByteDance.

## What It Does

- **Input:** Accepts pasted text, natural-language requests, and scripts in TXT, Markdown, DOCX, or PDF format.
- **Script analysis:** Automatically identifies characters, scenes, dialogue, actions, audio, and production requirements.
- **Shot breakdown:** Automatically breaks the content into generation-ready shots for Seedance 2.5.
- **Mode selection:** Automatically selects standard generation, long-video, video-extension, smart-editing, first-frame, or first-and-last-frame modes.
- **Asset planning:** Produces character and scene consistency rules, an asset list, and `@image/@video/@audio` mappings.
- **Ready-to-use prompts:** Generates shot-by-shot prompts ready to copy into Seedance 2.5.
- **Quality checks:** Checks duration, dialogue attribution, asset references, and continuity between shots.

## 安装

### 下载 ZIP

1. 点击仓库右上角的 **Code → Download ZIP**。
2. 解压下载文件。
3. 将其中的 `convert-script-to-seedance` 文件夹复制到 Codex 个人 Skills 目录：

Windows：

```text
%USERPROFILE%\.codex\skills\convert-script-to-seedance
```

macOS / Linux：

```text
~/.codex/skills/convert-script-to-seedance
```

4. 重新打开 Codex 或开始一个新任务。

### Git 克隆

```bash
git clone https://github.com/hjh836261459-cmd/seedance2.5-script-to-prompt-skill.git
```

然后把仓库里的 `convert-script-to-seedance` 文件夹复制到 `~/.codex/skills/`。

## 使用

上传剧本后直接说：

```text
用 $convert-script-to-seedance 把这个剧本转换成 Seedance 2.5 分镜提示词，并列出所需素材。
```

也可以输入自然语言：

```text
制作一条60秒竖屏悬疑短剧，两名角色，写实电影风格。请拆成 Seedance 2.5 分镜，保留全部对白，并保持人物外观一致。
```

Skill 也支持隐式触发，例如：

```text
把这个剧本转换成 Seedance 2.5 提示词。
```

## 默认输出

1. 转换摘要
2. 假设与待确认项
3. 素材清单
4. 全局一致性设定
5. 分镜计划
6. 可直接复制的逐镜提示词
7. 生成与拼接顺序
8. 风险与建议

## 来源说明

本 Skill 的参数、模式路由和提示词结构，依据 Seedance 2.5 官方使用手册整理并转化为可执行工作流。仓库不包含官方手册原文件，仅包含基于其内容总结的规则和模板。
