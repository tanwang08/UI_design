# UI设计 skill

将 [Anthropic frontend-design](https://github.com/anthropics/skills/tree/ca45fc496a3436251f191354091d557da31c15b5/skills/frontend-design) 改编为适合中文使用的 Codex 技能。

显示名称：**UI设计**。调用标识：`$ui-design`。支持界面设计、视觉改版、排版配色、交互文案、设计评审和前端实现；遵循用户需求与已有品牌规范。

## 调用示例

```text
使用 $ui-design，帮我设计一个亲子活动报名页，风格温暖明快，优先适配手机。
```

```text
使用 $ui-design，改进当前仪表盘的层级和排版，保留现有品牌色与组件库，并完成代码修改。
```

```text
使用 $ui-design，评审这个页面的视觉和交互，只给改进方案，暂不修改代码。
```

## 本地安装

在 Codex 中发送：

```text
请使用 skill-installer 安装 https://github.com/tanwang08/UI_design/tree/main/ui-design
```

也可以使用 Codex 自带的安装脚本：

```bash
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-installer/scripts/install-skill-from-github.py" \
  --repo tanwang08/UI_design --path ui-design
```

默认安装到 `~/.codex/skills/ui-design`，设置 `CODEX_HOME` 时则安装到该目录下的 `skills/ui-design`。安装完成后，从下一轮对话开始调用。若同名目录已经存在，安装器会停止，更新前应先保留本地改动。

## 文件与来源

- [`ui-design/SKILL.md`](ui-design/SKILL.md)：中文技能说明、工作方式及改编记录。
- [`ui-design/agents/openai.yaml`](ui-design/agents/openai.yaml)：Codex 显示名称和默认调用提示。
- [`ui-design/LICENSE.txt`](ui-design/LICENSE.txt)：上游 Apache-2.0 许可证，原样保留。

基于上游提交 `ca45fc496a3436251f191354091d557da31c15b5`，于 2026-11-06 改编。此仓库为中文适配版本，不是 Anthropic 官方中文版。同步的是当前适配版本，后续更新需重新比较与同步。
