# world-cup-alarm-2026

2026 世界杯观赛闹钟规划师。

本 Skill 基于你的个性化喜好，为你筛选值得熬夜的场次，帮你决定“哪场比赛值得定闹钟”，并创建“今夜值守简报”和“昨夜结果简报”两个自动化定时推送任务。

## 它能帮你做什么？

### 01 个性化推荐

告诉它你关注哪些球队或球员，比如阿根廷、梅西、日本队。后续所有推荐都会围绕你的偏好展开，不关心的比赛自动降级或过滤。

### 02 两个自动简报

- 每天 17:30 推送“今夜值守简报”：今晚几场、几点开球、哪场值得熬。
- 每天 09:00 推送“昨夜结果简报”：昨夜赛果 30 秒速览，你关注的球队发生了什么。

### 03 每场比赛自动打标

- 🔴 定闹钟：你关注的球队或球员出场，或强强对话、生死战。
- 🟡 看情况：建议睡觉，明早看集锦或结果。
- ⚪ 跳过：无关场次，不打扰。

### 04 随时对话查询

临时想问“今晚有球吗”“阿根廷下场什么时候”“这场值得看吗”，直接问 Codex，它会按北京时间给出结果。

## 安装

推荐使用 npx 一键安装：

```bash
npx world-cup-alarm-2026
```

安装完成后，重启 Codex，或在 Codex app 中使用 **Force Reload Skills**。

如果已经安装过旧版本，可以覆盖安装：

```bash
npx world-cup-alarm-2026 -- --force
```

如果你不想使用 npx，也可以直接 clone 到 Codex skills 目录：

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/PENGLEI8686/world-cup-alarm-2026.git ~/.agents/skills/world-cup-alarm-2026
```

之后更新：

```bash
cd ~/.agents/skills/world-cup-alarm-2026
git pull
```

## 使用

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
