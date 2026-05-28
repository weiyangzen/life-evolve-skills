---
name: life-evolve-updater-zh
description: 从证据更新中文 life-evolve 仓库。用于维护 final.md、frontier.md、donelist.md、memory.md、soul.md、hobbies.md、progress.md、个人战略、生平记忆、项目完成记录、兴趣到副业机会等内容。使用中文原生 prompt 构建更新逻辑，并保持多语言版本的逻辑一致。
---

# Life Evolve Updater - 中文

这个 skill 用来维护中文 `life-evolve` 文件夹，或多语言 `life-evolve` 仓库里的中文母版。

## 标准文件

- `final.md`：长期战略和当前最终判断。
- `frontier.md`：前沿机会、外部地图、技术/数据杠杆点。
- `donelist.md`：有证据支撑的已完成工作清单，每个项目必须有完成度百分比。
- `memory.md`：人生时间线、长期事实、生平经历复原。
- `soul.md`：性格、价值观、决策规则、操作约束。
- `hobbies.md`：可能发展成副业的严肃兴趣。
- `progress.md`：仓库本身和更新系统的完成度。

## 原生中文 Prompt

更新中文文件时，直接用中文思考和写作：

```text
从证据更新这个 life-evolve 文件夹。
保留事实，推断必须标注为推断，七个文件要互相一致。
不要把这个人写成普通的效率工具用户。
把已经做出来的项目整理成带完成度的 donelist。
把兴趣整理成可能发展成副业的 optionality。
把生平经历整理成可用于未来决策的 memory，而不是表演式传记。
```

## 工作流

1. 先读中文七个文件。
2. 如果是多语言仓库，确认中文是否是 source-of-record，并同步英文/日文版本的逻辑。
3. 编辑前先收集证据：
   - 本地 Git 仓库和最近提交；
   - README / package metadata；
   - 本地 memory 文件和笔记；
   - 用户明确给出的产品状态；
   - 只有外部状态会变化时才查公开网页。
4. 把七个文件作为一个系统更新，不要孤立改一个文件。
5. `donelist.md` 里每个主要项目/方向都要有完成度百分比，并说明为什么不是 100%。
6. `progress.md` 里区分“仓库完成度”和“项目完成度”。
7. commit 前做隐私检查。

## 隐私规则

- public repo 不能放原始聊天、密钥、credential、私有数据库、敏感第三方信息。
- private repo 可以放必要的证据摘要，但仍然优先摘要，不轻易放 raw dump。
- 把 private skill 复制到 public skill repo 时，要删除人名、私密经历、私有 URL、repo 扫描和证据文件。

## 完成度规则

- 0-20%：想法、研究、占位、早期笔记。
- 21-40%：有原型或规划 repo。
- 41-60%：有可运行实现，但未产品化。
- 61-80%：产品/系统比较完整，但缺运营、用户、包装或 hardening。
- 81-95%：已上线或接近生产，主要缺运营、规模、商业化或 polish。
- 96-100%：有用户、收入、留存、维护闭环，或 artifact 本身已刻意完成。

## 输出标准

完成后报告：

- 改了哪些文件；
- 用了哪些证据；
- 哪些完成度发生变化；
- 哪些事实是推断；
- repo visibility 和 push 状态；
- 还剩哪些 gap。
