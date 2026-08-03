# Seedance 2.5 Script to Prompt Skill

只需放入剧本或用自然语言描述创意，本 Skill 即可生成符合 Seedance 2.5 标准格式的提示词。本 Skill 基于 Seedance 2.5 官方使用手册整理。

Simply provide a script or describe your idea in natural language, and this skill will generate prompts in a standardized format optimized for Seedance 2.5. It is based on the official Seedance 2.5 user guide.

> 这是一个非官方社区项目，与即梦或字节跳动不存在隶属或背书关系。  
> This is an unofficial community project and is not affiliated with or endorsed by Jimeng or ByteDance.

## 能做什么 / What It Does

- **输入 / Input：** 接收粘贴文本、自然语言需求、TXT、Markdown、DOCX 或 PDF 剧本。 / Accepts pasted text, natural-language requests, and scripts in TXT, Markdown, DOCX, or PDF format.
- **内容解析 / Script analysis：** 自动识别角色、场景、对白、动作、声音和成片要求。 / Automatically identifies characters, scenes, dialogue, actions, audio, and production requirements.
- **自动拆镜 / Shot breakdown：** 自动拆分为适合 Seedance 2.5 生成的镜头。 / Automatically breaks the content into generation-ready shots for Seedance 2.5.
- **模式选择 / Mode selection：** 自动判断普通生成、超长视频、视频延长、智能编辑、首尾帧等模式。 / Automatically selects standard generation, long-video, video-extension, smart-editing, first-frame, or first-and-last-frame modes.
- **素材规划 / Asset planning：** 输出角色与场景一致性设定、素材清单以及 `@图/@视频/@音频` 映射。 / Produces character and scene consistency rules, an asset list, and `@image/@video/@audio` mappings.
- **标准提示词 / Ready-to-use prompts：** 输出可直接复制到 Seedance 2.5 的逐镜提示词。 / Generates shot-by-shot prompts ready to copy into Seedance 2.5.
- **质量检查 / Quality checks：** 检查时长、台词归属、素材引用和镜头衔接。 / Checks duration, dialogue attribution, asset references, and continuity between shots.

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
