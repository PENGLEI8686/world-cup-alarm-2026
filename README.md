# world-cup-alarm-2026

2026 World Cup alarm-planning Skill for Chinese football fans.

这个 Skill 面向中国国内用户，帮助用户判断 2026 世界杯哪些比赛值得定闹钟爬起来看，并输出中文观赛建议、闹钟清单和简报任务提示。

## What It Does

- 查询 2026 世界杯实时赛程和比分
- 将比赛时间统一换算为北京时间
- 按关注球队、关注球员、淘汰赛阶段和强强对话给比赛评级
- 输出 `定闹钟`、`看情况`、`跳过` 三类观赛建议
- 为支持自动化的平台生成今夜值守简报和昨夜结果简报

## Install

Clone this repository into your Codex user skills folder:

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/PENGLEI8686/world-cup-alarm-2026.git ~/.agents/skills/world-cup-alarm-2026
```

Then restart Codex, or use **Force Reload Skills** in the Codex app.

## Usage

Ask Codex in Chinese:

```text
启用世界杯闹钟
今晚有什么比赛值得看？
世界杯定闹钟
昨晚世界杯谁赢了？
```

You can also explicitly invoke the skill by mentioning:

```text
$world-cup-alarm-2026
```

## Requirements

This Skill needs a Codex environment with internet search access, because World Cup schedules, kickoff times, and match results must be checked live. It should not answer from memory.

Automation support is optional. If the current Codex surface supports automations, the Skill can help create evening and morning World Cup briefings. If not, it will still provide manual viewing advice in the current conversation.

## Files

- `SKILL.md`: Main Skill instructions
- `references/timezone-table.md`: 2026 host-city timezone conversion table

## License

MIT
