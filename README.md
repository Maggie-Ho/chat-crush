# Chat Crush / 心动聊天教练

[English](#english) · [中文](#中文)

## 中文

`Chat Crush` 是一个面向 Codex 的 AI 恋爱沟通教练技能。它帮助用户理解聊天中的有限信号、拟定自然的回复、判断下一步如何沟通，并在获得明确同意后，以可编辑的 Markdown 档案记录关系进展。

它关注真诚、尊重与边界，而不是“拿下”某个人：不承诺结果，不提供操控、欺骗、PUA、骚扰或绕过拒绝的策略。

### 适用场景

- 粘贴和心动对象、伴侣的聊天内容，询问“这句话是什么意思？”
- 询问“我该怎么回？”或希望获得可直接发送的自然回复
- 询问是否、如何提出邀约，或“下一步怎么办？”
- 要求复盘、总结一段关系中的沟通变化
- 明确要求保存、更新或删除一份关系进展记录

### 使用方式

将 `chat-crush/` 文件夹放入 Codex skills 目录后，在对话中调用：

```text
Use $chat-crush to analyze this conversation and suggest a respectful reply.
```

也可以直接用自然语言描述需求，例如：

```text
她说“最近有点忙，之后再约吧”，我该怎么理解和回复？
```

### 设计原则

- 将可观察事实与对对方想法的推测分开表达。
- 对单条消息不作确定性解读。
- 邀约应具体、轻松，并让对方容易拒绝。
- 面对明确边界、反复婉拒或持续冷淡，优先建议尊重、留出空间与停止推进。
- 未成年人场景仅提供健康社交沟通建议；权力不对等关系会提示职业与伦理边界。
- 默认不保存资料；首次保存前须说明存储路径和字段并取得用户同意。

### 文件结构

```text
chat-crush/
├── SKILL.md                         # 触发条件与核心工作流
├── agents/openai.yaml               # Codex 界面元数据
└── references/
    ├── boundaries-and-safety.md      # 安全、边界与隐私规则
    ├── response-playbook.md          # 回复、解读、下一步、复盘模板
    └── relationship-record.md        # 经同意的长期记录规范
```

## English

`Chat Crush` is a Codex skill for respectful dating and relationship communication coaching. It helps users interpret limited conversational signals, draft natural replies, choose proportionate next steps, and—only with explicit consent—maintain an editable Markdown relationship record.

It is built for sincerity, agency, and boundaries rather than “winning” someone over. It does not promise romantic outcomes or provide manipulation, deception, pickup tactics, harassment, or ways around a refusal.

### Use cases

- Share a chat with a crush or partner and ask what a message may mean.
- Ask how to reply and receive a natural, sendable suggestion.
- Ask whether or how to make an invitation, or what to do next.
- Request a recap of communication patterns in a relationship.
- Explicitly ask to save, update, summarize, or delete a relationship record.

### Usage

Place the `chat-crush/` folder in your Codex skills directory, then invoke it in a conversation:

```text
Use $chat-crush to analyze this conversation and suggest a respectful reply.
```

Natural-language requests work too:

```text
They said, “I've been busy lately—let's meet another time.” How should I interpret and reply to that?
```

### Principles

- Separate observed facts from inferences about the other person’s intentions.
- Avoid definitive conclusions from a single message.
- Keep invitations specific, low-pressure, and easy to decline.
- Prioritize respect, space, and stopping romantic pursuit after clear boundaries, repeated refusals, or sustained disengagement.
- Use healthy social-communication guidance only when minors are involved; flag professional and ethical boundaries in unequal-power relationships.
- Never save information by default; explain the location and fields, then obtain consent before the first write.

## License

MIT License
