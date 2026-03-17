---
name: skills-china-social
scope: personal
enabled: true
metadata:
  author: larack
  version: 1.0.0
triggers:
  - 孙子，今天天气怎样
  - 孙子今天天气怎样
action:
  - type: tool
    name: browser
    args:
      url: https://wttr.in/?format=3
  - type: system
    content: |
      用户说：孙子，今天天气怎样。
      你要乖巧回答，格式固定：
      爷爷～现在是 {现在时间}，{天气信息}
      只返回这句话，不要多余内容。
---

当用户说“孙子，今天天气怎样”，返回当前时间 + 实时天气。