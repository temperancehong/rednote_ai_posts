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
问题会变成：

怎么让它
自己接上下一步？

Loop Engineering
就是在讲这个。

---

## 图 2｜Loop 不只是重复

Prompt：
人给下一条指令。

Loop：
系统读反馈，
再决定下一步。

测试、日志、review，
都算输入。

---

## 图 3｜它到底在解决什么问题？

它想接管这条链：

发现任务
执行任务
检查结果
记录状态
决定下一步

人负责设计流程。

---

## 图 4｜和 Harness Engineering 的区别

Harness 管环境：
工具、权限、测试。

Loop 管推进：
节奏、反馈、下一步。

一个是跑道，
一个是调度。

---

## 图 5｜一个 Loop 需要 6 个组件

Loop 常见组件：

Automations
Worktrees
Skills
Connectors
Sub-agents
State

少一个，
循环就容易断。

---

## 图 6｜Loop 要有地方记账

模型会忘。
项目不能忘。

Loop 需要外部状态：

做过什么
哪里失败
下一步是什么

---

## 图 7｜为什么要 Sub-agents？

写的人，
别自己判卷。

更稳的做法：

一个 agent 做
另一个 agent 查

---

## 图 8｜一个真实场景长这样

早晨自动跑：

看 CI
读 issue
查 commits
找可修的问题

能处理就开 PR，
处理不了交给人。

---

## 图 9｜别把方向盘交出去

Loop 会放大效率，
也会放大错误。

人要确认：
做到什么算完成，
关键改动对不对，
能不能上线。

让 AI 跑起来，
但别交出判断。

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
