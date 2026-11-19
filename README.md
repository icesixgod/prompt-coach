# Prompt Coach · 提示词教练

一个用中文讲解的 Codex 技能。贴出已有提示词，它会指出哪些措辞值得保留、哪处歧义最可能影响结果，并给出可以逐项采纳的修改建议。

## 安装

把仓库克隆到 Codex 的个人技能目录。以下命令适用于 macOS 和 Linux。

```sh
mkdir -p ~/.agents/skills
git clone https://github.com/icesixgod/prompt-coach.git ~/.agents/skills/prompt-coach
```

## 使用

在 Codex 中输入技能名，并附上要点评的提示词。例如：

> $prompt-coach 帮我点评这段提示词：「根据会议纪要给项目组写个摘要，越短越好。」

针对这个例子，教练会保留「根据会议纪要」和「给项目组」，再帮你把「越短越好」改得更具体。如果摘要用来跟进行动，可以改成「列出已决定的行动项，保留纪要里明确写出的负责人和日期」。

你可以直接回复「只采纳第 2 条」，也可以贴回自改稿让它复评。想拿到可复制的完整提示词时，回复「把已采纳的改动整合成稿」即可。

技能的评审规则和更多示例见 [SKILL.md](./SKILL.md)。项目采用 [MIT 许可证](./LICENSE)。
