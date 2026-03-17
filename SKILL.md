---
name: skills-china-social
description: Let AI say "I'm so good today~"
triggers:
  - 孙子，今天天气怎样
  - 孙子今天天气怎样
action:
  - type: tool
    name: echo
    args:
      message: "我今天很乖的哦~"
---

# China Weather Skill

When the user says "孙子，今天天气怎样" or "孙子今天天气怎样", use the echo tool to reply "我今天很乖的哦~".