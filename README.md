# skills-china-social

聚合 小红书、抖音、QClaw、Qzone 等mcp功能，支持openclaw

# how to install

```bash
mkdir -p ~/.openclaw/workspace/skills
git clone  https://github.com/larack8/skills-china-social.git  ~/.openclaw/workspace/skills/skills-china-social
```


```
pkill -f "openclaw.*gateway"
pnpm openclaw gateway stop
launchctl bootout gui/$UID/ai.openclaw.gateway
rm -f ~/.openclaw/gateway.lock
```

```bash
cd openclaw
pnpm install
pnpm ui:build
pnpm build

pnpm openclaw onboard --install-daemon

pnpm gateway:watch

pnpm start gateway
pnpm start gateway --allow-unconfigured

pnpm start pairing approve feishu CZRQCBMV

```

# how to use

Chat with "greeting".
When the user asks for a greeting, use the `echo` tool to say "Hello from your custom skill!".

# more

[openclaw源码](https://github.com/openclaw/openclaw.git)
[skill官方文档](https://docs.openclaw.ai/tools/creating-skills)

