# 小红书图文草稿：Loop Engineering 是什么？

## 元信息

- Post title: Loop Engineering 是什么？AI Agent 用久后会遇到的新问题
- Post draft date: 2026-07-05
- Original article: [Loop Engineering](https://addyosmani.com/blog/loop-engineering/)
- Original author: Addy Osmani
- Original publish date: 2026-06-07
- Source language: English
- Draft language: Chinese
- Format: Xiaohongshu carousel / 一图一个观点

---

## 图 1｜封面

AI Agent 用久了，
会遇到一个新问题：

怎么让它自己接上下一步？

Loop Engineering
开始被认真讨论了。

---

## 图 2｜Loop 不只是重复

Prompt Engineering：
人给下一条指令。

Loop Engineering：
系统读反馈，
再安排下一步。

测试结果、运行日志、
草稿、review comment，
都会变成新的输入。

---

## 图 3｜它到底在解决什么问题？

以前用 AI Agent：
人一直在旁边推进。

Loop 想接管的是这条链：

发现任务
执行任务
检查结果
记录状态
决定下一步

你的角色会更像
工作流设计者。

---

## 图 4｜和 Harness Engineering 的区别

Harness Engineering 关注的是：
agent 跑在哪里。

Loop Engineering 关注的是：
系统怎么往前走。

Harness 给工具和边界。
Loop 安排节奏和下一步。

---

## 图 5｜一个 Loop 需要 6 个组件

能跑起来的 Loop，
通常靠这 6 件事：

Automations：定时跑
Worktrees：隔离修改
Skills：写下经验
Connectors：接工具
Sub-agents：分工查
State：记进展

---

## 图 6｜Loop 要有地方记账

模型会忘。
项目不能忘。

Loop 需要外部状态：

做过什么
哪里失败
什么还没关

明天再跑，
才能接着今天走。

---

## 图 7｜为什么要 Sub-agents？

写的人，
不适合自己判卷。

更稳的结构：

一个 agent 做
另一个 agent 查

Loop 越自动，
越需要独立验证。

---

## 图 8｜一个真实场景长这样

一个早晨自动跑的 Loop：

看 CI
读 issue
查 commits
找可修的问题

然后修复、测试、开 PR。

处理不了的，
再交回给人。

---

## 图 9｜别把方向盘交出去

Loop 会放大效率，
也会放大错误。

工程师仍然要负责：

完成标准
关键 review
理解变化

Build the loop.
Stay the engineer.

让 AI 跑起来，
但别把判断交出去。

---

## 小红书标题备选

1. AI Agent 用久后，我开始关心 Loop 了
2. Loop Engineering：AI 工作流的新关键词
3. 只会 prompt，可能很快不够用了
4. 让 AI 持续推进工作的设计方法

---

## 配文 Caption

最近读到 Addy Osmani 写的 Loop Engineering，里面讲到一个很实际的变化：

以前大家很关注 prompt 怎么写。
这篇文章把问题往前推了一步：
怎样设计一个能持续工作的 AI 循环？

一个好的 Loop，会把测试结果、日志、草稿、review comment 这些中间产物重新喂回流程里。
下一步怎么走，先看反馈。

这也是为什么未来的 AI 工作流里，记忆、验证、状态、工具连接、sub-agent 会越来越重要。

AI 可以跑起来，
但判断力还是要留在人这里。

#AI工具 #LoopEngineering #PromptEngineering #AI工作流 #Agent #效率工具 #程序员 #产品经理
