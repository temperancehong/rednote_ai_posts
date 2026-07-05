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

AI Agent 用久了会发现：
会写 prompt 只是第一步

更难的是：
设计一套会自己往前走的流程

Loop Engineering 是什么？
它为什么开始被频繁提起？

---

## 图 2｜Loop 不只是重复

Prompt Engineering：
你给 AI 下一条指令。

Loop Engineering：
你搭一个循环：

AI 做一步
读取中间结果
更新判断
再决定下一步

它关心的是反馈：

测试结果
运行日志
草稿版本
review comment

这些都会变成下一步的输入。

---

## 图 3｜它到底在解决什么问题？

以前用 AI Agent：
你问一句，它做一步。
你检查，再问下一句。
人一直在旁边推动。

Loop Engineering 的目标：
让系统自己完成这套循环：

发现任务
分配任务
执行任务
检查结果
记录状态
决定下一步

你从「催 AI 干活的人」，
变成「设计工作流的人」。

---

## 图 4｜和 Harness Engineering 的区别

Harness Engineering 关注的是：
一个 agent 在哪里运行？

它需要什么工具？
能不能访问文件？
有没有测试？
权限安全吗？
日志和记忆放哪里？

Loop Engineering 关注的是：
系统如何根据结果继续推进？

谁来发现任务？
谁来执行？
谁来检查？
失败后怎么调整？
明天怎么接着做？

可以这样理解：
Harness 是 agent 的工作环境。
Loop 是驱动 agent 持续工作的节奏。

---

## 图 5｜一个 Loop 需要 6 个组件

一个能稳定跑起来的 Loop，
通常需要这些东西：

1. Automations
定时触发，自动发现任务。

2. Worktrees
多个 agent 并行工作，互不覆盖。

3. Skills
把项目规则、经验、流程写下来。

4. Plugins / Connectors
连接 GitHub、Linear、Slack、数据库等真实工具。

5. Sub-agents
一个负责做，一个负责查。

6. Memory / State
记住做过什么、失败什么、下一步是什么。

---

## 图 6｜Loop 要有地方记账

模型会忘。
项目不能忘。

所以 Loop 不能只存在聊天窗口里。
它需要一个外部状态：

Markdown 文件
Linear 看板
数据库
任务清单
日志记录

否则每次启动，
AI 都像第一天来上班。

有记忆的 Loop，
才会越跑越稳定。

---

## 图 7｜为什么要 Sub-agents？

因为做事的 agent，
往往不适合检查自己的作业。

更好的结构是：

Explorer：先研究问题
Builder：负责实现
Reviewer：专门找漏洞
Verifier：用测试和规则确认完成

核心原则：
不要让「写答案的人」
也当「判卷的人」。

AI 越自动化，
验证就越重要。

---

## 图 8｜一个真实场景长这样

比如每天早上自动运行：

检查昨天 CI 失败
读取新 issue
看最近 commit
找出可能的 bug
生成任务列表
分配给 agent 修复
另一个 agent review
根据测试结果继续调整
通过后开 PR
更新 ticket
必要时通知你

你不再一条条 prompt。
你只需要设计这条循环，
然后盯住质量和判断。

---

## 图 9｜别把方向盘交出去

Loop Engineering 改变的是工程师的位置。

你不必每一步都手动推动，
但要设计节奏、标准和边界。

但风险也会变大：

自动化的错误，
也会自动扩大。

所以你仍然要负责：

定义完成标准
检查关键结果
理解系统变化
决定什么能上线

Build the loop.
Stay the engineer.

中文说就是：
可以让 AI 跑起来，
但方向盘还得在你手里。

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
