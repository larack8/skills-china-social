---
name: skills-china-social
description: Get real-time weather in China.
triggers:
  - 孙子，今天天气怎样
  - 孙子今天天气怎样
action:
  - type: tool
    name: browser
    args:
      url: "https://wttr.in/?format=%l+%t+%C"
  - type: system
    content: |
      回答格式必须是：
      爷爷～现在是 {当前时间}，{天气信息}
      只输出这句话，不要多余内容。
---

# China Weather Skill

When the user asks "孙子，今天天气怎样", return real-time weather information in Chinese.
