# Yang Weibo & Book Notes

> AI 很容易把观点微博写成口号，把读书笔记写成摘要。这个 Skill 让创作从事实出发，分析机制与现实约束，再给出克制、清楚的个人判断。
>
> Turn source material into thoughtful Chinese Weibo posts and book notes grounded in facts, mechanisms, constraints, and measured judgment.

[![Stars](https://img.shields.io/github/stars/tianyayu6/yang-weibo-book-notes?style=flat-square)](https://github.com/tianyayu6/yang-weibo-book-notes/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/tianyayu6/yang-weibo-book-notes?style=flat-square)](https://github.com/tianyayu6/yang-weibo-book-notes/commits/main)
[![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)

```bash
npx skills add tianyayu6/yang-weibo-book-notes
```

**[中文](#中文) | [English](#english)**

## 中文

### 它解决什么问题

这个 Skill 来自微博账号“阅读思考写作-每日不坠”的公开文章样本。它不机械复制旧文句子，而是提炼一套可迁移的创作方法：

- 从具体事实、亲历或书中问题起笔
- 分析制度、商业、技术、情感与利益约束
- 区分已知事实、合理推断和个人感受
- 主动呈现反面可能与结论边界
- 用朴素、连续、克制的中文完成判断

它分别处理短微博、观点微博、事件评论、转发语和读书笔记，不把不同体裁压进同一个模板。

### 输出预览

给它一则新闻和你的初步判断，它不会直接制造一个激烈立场，而会先梳理：发生了什么、哪些信息仍不确定、各方承担什么成本、现有机制为何形成，最后落在一个有限但明确的结论上。

给它书名、划线和阅读感受，它会围绕书中最值得继续追问的问题组织文章，而不是按章节复述内容或虚构书中案例。

### 安装

1. 确认本机已安装 Node.js 与 npm：

   ```bash
   node --version
   npm --version
   ```

2. 安装 Skill：

   ```bash
   npx skills add tianyayu6/yang-weibo-book-notes
   ```

3. 查看可发现的 Skill：

   ```bash
   npx skills add tianyayu6/yang-weibo-book-notes --list
   ```

### 你可以这样说

- “使用 `$yang-weibo-book-notes`，把这些材料写成一篇 600 字的观点微博。”
- “根据我的划线和批注，写一篇《某书》读书笔记，不要写成内容摘要。”
- “把这段转发语改得更像我的表达，保留不确定性，不要制造金句。”
- “核验这则新闻，再写一篇事件评论，区分事实和推测。”

### 前置条件

- [ ] 使用支持 Agent Skills 的 Codex、Claude Code 或兼容工具
- [ ] 已安装 Node.js；可从 [nodejs.org](https://nodejs.org/) 获取
- [ ] 写时效性事件评论时，允许 Agent 查询可靠来源
- [ ] 写读书笔记时，尽量提供划线、批注、摘录或自己的感受

### 设计原则

- **原创优先**：复现思考方式，不照抄历史文本。
- **事实优先**：无法核验的数字、引语、情节和作者主张不得补写。
- **体裁分离**：微博追求信息密度，读书笔记围绕一个问题持续展开。
- **克制判断**：允许有立场，但不把推测包装成事实。
- **直接交付**：默认输出可发布成稿，不先堆砌创作说明。

### 限制

- 当前风格画像主要依据公开可访问的近期微博、AI 使用回顾和一篇完整读书笔记，不能替代作者本人对试稿的持续修正。
- 只有书名而没有原书材料时，Skill 会降低断言强度，不会假装已经通读。
- 它不会自动知道读书笔记序号；未提供序号时不会自行续号。
- 新闻、数据和人物近况会变化，发布前仍应检查引用和时效事实。

### 常见问题

| 问题 | 解决方法 |
|---|---|
| 输出像普通 AI 文案 | 提供一段自己的判断、亲历或批注，并明确希望保留的核心观点。 |
| 读书笔记过于概括 | 提供划线、目录、书中案例或阅读时真正困惑的问题。 |
| 事件评论写得太确定 | 要求逐项标出已知事实、推断和无法确认的信息，再生成成稿。 |
| Skill 没有触发 | 在请求中明确写出 `$yang-weibo-book-notes`。 |
| `npx skills` 找不到 Skill | 更新 Node.js/npm 后重新运行安装命令，并用 `--list` 检查。 |

### 画像来源

风格画像依据账号公开内容提炼，来源与使用限制记录在 [`references/source-basis.md`](references/source-basis.md)。

## English

This Agent Skill creates and revises Chinese Weibo posts and book notes in a restrained, reasoning-led voice. It focuses on the transferable process behind the writing rather than copying distinctive sentences from previous posts.

### What it does

- Starts from concrete facts, lived experience, or a central question from a book
- Explains incentives, institutions, technology, emotion, and practical constraints
- Separates verified facts, inference, and personal judgment
- Includes counterarguments and limits before reaching a conclusion
- Supports short posts, event commentary, repost captions, and long-form book notes

### Install

```bash
npx skills add tianyayu6/yang-weibo-book-notes
```

### Example prompts

- "Use `$yang-weibo-book-notes` to turn these materials into a 600-character Chinese Weibo post."
- "Write a book note from my highlights and comments without summarizing every chapter."
- "Verify this news item, then draft a measured event commentary that separates facts from inference."

### Limitations

The current voice profile is based on publicly accessible samples and should evolve with direct author feedback. The Skill does not invent quotations, book details, personal experience, or book-note sequence numbers.

## License

[MIT](LICENSE)
