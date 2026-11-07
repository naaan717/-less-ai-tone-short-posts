# 短帖去 AI 味自查 · less-ai-tone-short-posts

一份给中文短帖用的去 AI 味清单，适合小红书、朋友圈、X 中文帖这类 500 字以内的内容。写完之后、发出之前，让 AI 照着它逐句自查，只改真正有区分度的那几种写法，其余一律不动。

## 和原版有什么不同

规则来自 [lieflat-less-ai-tone](https://github.com/larashero3-dotcom/lieflat-less-ai-tone)。原作者拿五个模型写的文章和人类文章对比了两轮，筛出 AI 确实比人用得多的写法，也推翻了不少流传很广的「去 AI 味」说法。

原版是给长文做的，检测脚本少于 500 个汉字直接不工作，流程也比较重。这个版本只保留规则本身：

- 去掉了脚本和分级报告，一份 `SKILL.md` 就能用
- 只留下 8 条要改的写法和一份「别改」清单
- 强调最小改动：事实、限定词、语气、结构都不动
- 例子换成了中文短帖

## 怎么用

**Claude Code / 支持 Skills 的 Agent**：把整个文件夹放进 `~/.claude/skills/`（或项目里的 `.claude/skills/`），写完帖子后说一句「按 less-ai-tone-short-posts 自查一下」。

**Cursor**：把 `SKILL.md` 的内容放进 `.cursor/rules/` 下的一条规则，或者对话里直接 @ 这个文件。

**ChatGPT / Gemini / 其他聊天工具**：把下面这段连同 `SKILL.md` 全文一起发过去：

```
下面是一份中文短帖去 AI 味的自查规则。请按规则逐句检查我接着贴的帖子：
只改命中规则的地方，每处最小改动，事实、数字、限定词、标题、代码块和话题标签都不要动。
先给改后全文，再用一行说明改了哪几类。
（规则全文）
（我的帖子）
```

## 示例

[examples/before-after.md](./examples/before-after.md) 是一篇小红书帖的改前改后对照。

## 许可

沿用原项目的 [CC BY-NC 4.0](./LICENSE)：可以自由使用、修改、转载，需保留原作者 shiujan 及原仓库署名，不可商用。
