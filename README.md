# World Cup Alarm 2026 / 2026 世界杯观赛闹钟规划师

[中文](#中文) | [English](#english)

## 中文

2026 世界杯观赛闹钟规划师，帮你决定“哪场比赛值得定闹钟”。

本 Skill 基于你的球队和球员偏好，筛选值得熬夜的场次，输出手机闹钟清单，并可创建“今夜值守简报”和“昨夜结果简报”两个自动化定时推送任务。

### 它能帮你做什么

- **个性化推荐**：告诉它你关注哪些球队或球员，比如阿根廷、梅西、日本队；后续推荐围绕你的偏好展开。
- **两个自动简报**：每天 17:30 推送“今夜值守简报”，每天 09:00 推送“昨夜结果简报”。
- **每场比赛自动打标**：🔴 定闹钟、🟡 看情况、⚪ 跳过，并附一句话理由。
- **随时对话查询**：临时问“今晚有球吗”“阿根廷下场什么时候”“这场值得看吗”，按北京时间直接给结果。

### 安装

推荐使用 npx 一键安装：

```bash
npx github:PENGLEI8686/world-cup-alarm-2026
```

安装完成后，重启 Codex，或在 Codex app 中使用 `Force Reload Skills`。

覆盖安装：

```bash
npx github:PENGLEI8686/world-cup-alarm-2026 -- --force
```

也可以直接 clone 到 skills 目录：

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/PENGLEI8686/world-cup-alarm-2026.git ~/.agents/skills/world-cup-alarm-2026
```

### 使用示例

```text
使用 $world-cup-alarm-2026，启用世界杯闹钟，我关注阿根廷和日本队。
```

```text
今晚有什么比赛值得看？帮我列闹钟清单。
```

### 注意

本 Skill 需要联网搜索能力，因为世界杯赛程、开球时间和比分必须实时核对。自动化推送能力是可选项；如果当前 Agent 环境不支持定时任务，仍可在对话中手动查询赛程和值守建议。

## English

World Cup Alarm 2026 helps you decide which 2026 FIFA World Cup matches are worth waking up for.

The Skill uses your favorite teams and players to rate matches, build phone alarm lists, and optionally create two scheduled briefings: an evening “tonight watch briefing” and a morning “last night results briefing.” Times are optimized for Beijing time by default, because many matches in the U.S., Canada, and Mexico will happen overnight for China-based fans.

### What It Helps With

- **Personalized match recommendations**: tell it which teams or players you follow.
- **Two scheduled briefings**: evening watch briefing and morning results briefing.
- **Match labels**: 🔴 wake up, 🟡 maybe skip and watch highlights, ⚪ skip.
- **Ad-hoc queries**: ask “Any games tonight?”, “When is Argentina’s next match?”, or “Is this match worth watching?”

### Installation

Recommended one-line install:

```bash
npx github:PENGLEI8686/world-cup-alarm-2026
```

After installation, restart Codex or use `Force Reload Skills` in the Codex app.

To overwrite an existing installation:

```bash
npx github:PENGLEI8686/world-cup-alarm-2026 -- --force
```

You can also clone the repository directly:

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/PENGLEI8686/world-cup-alarm-2026.git ~/.agents/skills/world-cup-alarm-2026
```

### Example Prompts

```text
Use $world-cup-alarm-2026 to set up my World Cup watch planner. I follow Argentina and Japan.
```

```text
Which World Cup matches tonight are worth waking up for? Give me an alarm list.
```

### Note

This Skill requires live web search because schedules, kickoff times, and match results must be verified in real time. Automation support is optional; without it, the Skill still works for manual match planning in conversation.
