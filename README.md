# AI Skills

我的公开 AI Skill 合集。每个 Skill 都放在 `skills/<skill-name>/`，可以单独安装。

## 已发布的 Skill

### [AI 博主选题](skills/ai-creator-topics/SKILL.md)

为 AI 内容创作者寻找、核实并排序适合拍成短视频或图文的早期选题。有账号主页时会先分析视频和表达风格；没有主页时按“一个新鲜的 AI 用法，普通人今天能拿它做什么”筛选。安装或首次使用后，会询问是否需要每日推送；只有用户确认时间后才设置定时任务。

## Codex

在 Codex 中说：

> 安装这个 Skill：https://github.com/Lin-QuQ/codex-skills/tree/main/skills/ai-creator-topics

也可以使用内置安装脚本：

```bash
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-installer/scripts/install-skill-from-github.py" \
  --repo Lin-QuQ/codex-skills \
  --path skills/ai-creator-topics
```

安装后下一轮对话即可使用。

## 豆包工作

在豆包工作的「技能・连接器・伙伴」中，使用新建或导入技能的入口，导入 [Skill 包](downloads/ai-creator-topics.zip) 或 `skills/ai-creator-topics/SKILL.md`。也可以先把 [SKILL.md](skills/ai-creator-topics/SKILL.md) 链接发给豆包工作，让它按文件内容执行；这种方式是否会保存为可重复调用的技能，以当前客户端显示为准。豆包工作支持自建、导入本地技能文件和定时任务，具体入口与权限可能因账号及客户端而异。参见[豆包工作官方介绍](https://www.feishu.cn/content/article/7677519271848610746)。

如果你使用的是普通豆包聊天入口，找不到技能导入入口时，可以把 `SKILL.md` 的内容作为提示词发给它做一次性选题。这样不等于已经安装 Skill，也不会自动产生每日推送。

## WorkBuddy

下载 [WorkBuddy 导入包](downloads/ai-creator-topics-workbuddy.zip)，在 WorkBuddy「专家・技能・连接器 → 技能 → 添加技能」中上传。这个 ZIP 的根目录直接包含 `SKILL.md`，并按[WorkBuddy 官方格式](https://open.workbuddy.cn/docs/skill)补齐了中英文描述、版本和作者；[源文件在这里](platforms/workbuddy/ai-creator-topics/SKILL.md)。WorkBuddy 的[客户端说明](https://cloud.tencent.com/document/product/1831/134432)支持导入本地 Skill 包；[自动化说明](https://cloud.tencent.com/document/product/1831/134399)支持在定时任务中选择 Skill 和结果推送方式。这里提供的是客户端导入包，尚未提交到 WorkBuddy 技能市场。

## 每日推送

Skill 首次使用时会先询问是否有账号主页，再确认是否需要每日推送和具体时间。只有用户确认后，才会尝试使用当前平台的定时任务功能；若无法代为创建，会说明未设置成功，并给出可复制的任务提示词。各平台的推送位置以其自动化功能实际支持的选项为准。
