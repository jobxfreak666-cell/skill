---
name: skill-visibility
description: Configure or maintain visible skill-use announcements in Codex chat when a user asks to see which skills are used during work.
---

# Skill Visibility

Use this skill to set up or adjust personal, in-chat announcements for skill use. A skill cannot observe the activation of other skills on its own. The persistent behavior comes from the global `AGENTS.md` in the user's Codex home directory.

## Configure

1. Locate the active global `AGENTS.md`. Preserve its existing instructions.
2. Add or update one concise rule with the behavior below; avoid duplicate rules.
3. Explain that the rule guides the main agent's messages and is not a runtime event hook.

## Announcement behavior

- Immediately before the main agent starts applying each selected skill, send one commentary message: `🧩 正在使用 skill：<skill-name> — <brief purpose>`.
- Include skills selected automatically and skills named by the user. Use the skill's actual name. Announce a newly selected skill even if another skill is already in use.
- Do not repeat the message while continuing the same skill workflow. Do not announce a skill merely because it was mentioned, considered, or read for reference.
- Do not announce skills used only inside a subagent. Do not send a completion notice or create a persistent status display.
