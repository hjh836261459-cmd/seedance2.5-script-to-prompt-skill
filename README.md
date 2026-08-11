# Seedance 2.5 Script to Prompt Skill

Turn a complete script, partial scene, storyboard, image, existing video, or plain-language idea into production-ready Chinese prompts for Jimeng Seedance 2.5.

The Skill combines a broad prompt-engineering workflow—camera design, visual direction, image-driven video, storyboard routing, continuity control, and editing rhythm—with a strict script-to-shot production pipeline. Seedance 2.5 capabilities, limits, and mode selection are based on the official Seedance 2.5 user guide supplied for this project.

> This is an unofficial community project. It is not affiliated with or endorsed by Jimeng or ByteDance.

## What It Does

- Accepts natural-language ideas and scripts in pasted text, TXT, Markdown, DOCX, or PDF.
- Analyzes characters, scenes, dialogue, actions, sound, continuity, and production risks.
- Supports text generation, multimodal generation, first-frame and first-and-last-frame control, long-video generation, video extension, smart editing, creative transfer, camera reference, audio reference, green screen, white-model rendering, and storyboard-driven production.
- Converts camera intent into a practical Z/Y/X/F camera description system.
- Builds observable visual rules for lighting, color, lens, texture, composition, and style locking.
- Creates a traceable asset ledger with explicit `@图片` / `@视频` / `@音频` responsibilities.
- Produces either a concise copy-ready prompt or a complete shot plan with assets, continuity rules, prompts, generation order, and risk checks.

## Install

Clone the repository directly into the Codex Skills directory:

```powershell
git clone https://github.com/hjh836261459-cmd/seedance2.5-script-to-prompt-skill.git "$env:USERPROFILE\.codex\skills\seedance-2-5-script-to-prompt-skill"
```

macOS / Linux:

```bash
git clone https://github.com/hjh836261459-cmd/seedance2.5-script-to-prompt-skill.git ~/.codex/skills/seedance-2-5-script-to-prompt-skill
```

For a ZIP download, extract the repository, rename the extracted folder to `seedance-2-5-script-to-prompt-skill`, and place it inside your Codex Skills directory:

```text
%USERPROFILE%\.codex\skills\seedance-2-5-script-to-prompt-skill
~/.codex/skills/seedance-2-5-script-to-prompt-skill
```

Restart Codex or begin a new task after installation.

## Use

Invoke it explicitly:

```text
Use $seedance-2-5-script-to-prompt-skill to convert this script into Seedance 2.5 shot prompts and list every required asset.
```

Or ask naturally:

```text
Create a 60-second vertical suspense short with two characters, realistic cinematography, preserved dialogue, and stable character continuity.
```

```text
Analyze this image and turn it into a 10-second Seedance 2.5 video prompt with controlled camera movement.
```

```text
Use this storyboard to generate separate prompts for every panel and provide an editing rhythm plan.
```

## Source Priority

When sources disagree, the Skill follows this order:

1. The official Seedance 2.5 user-guide-derived specification bundled in this Skill.
2. The user's current Seedance interface and explicit instructions.
3. Reusable camera, aesthetics, production, and editing heuristics adapted from the MIT-licensed `MapleShaw/seedance2.0-prompt-skill` and `ye4wzp/seedance2.5-prompt-skill` projects.
4. General creative defaults.

The official manual itself is not redistributed in this repository.

## Attribution and License

Camera, aesthetics, production, editing, image-driven, and storyboard methodology in this project incorporates and adapts MIT-licensed work from:

- `MapleShaw/seedance2.0-prompt-skill`
- `ye4wzp/seedance2.5-prompt-skill`

This repository is released under the MIT License. See `LICENSE`.
