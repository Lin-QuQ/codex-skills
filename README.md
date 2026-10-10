# Codex Skills

我的公开 Codex Skill 合集。每个 Skill 都放在 `skills/<skill-name>/`，可以单独安装。

## 已发布的 Skill

### [AI 博主选题](skills/ai-creator-topics/SKILL.md)

为 AI 内容创作者寻找、核实并排序适合拍成短视频或图文的早期选题。有账号主页时会先分析视频和表达风格；没有主页时按“一个新鲜的 AI 用法，普通人今天能拿它做什么”筛选。安装或首次使用后，会询问是否需要每日推送；只有用户确认时间后才设置定时任务。

## 安装到 Codex

在 Codex 中说：

> 安装这个 Skill：https://github.com/Lin-QuQ/codex-skills/tree/main/skills/ai-creator-topics

也可以使用内置安装脚本：

```bash
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-installer/scripts/install-skill-from-github.py" \
  --repo Lin-QuQ/codex-skills \
  --path skills/ai-creator-topics
```

安装后下一轮对话即可使用。定时推送需要当前环境支持定时任务，并由用户确认是否启用以及推送时间。
