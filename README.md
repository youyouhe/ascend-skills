# ascend-skills

Claude Code skills：**野心与认知升维架构师**。在动手执行任务之前，先从「高度、深度、广度、极限」四个维度解构并升维任务，再询问用户选择停留的高度。

| Skill | 调用 | 特点 |
|---|---|---|
| `ascend` | `/ascend 任务` | 原版四模块，可被自然语言自动触发 |
| `ascend-v1` | `/ascend-v1 任务` | 强化版：反套话铁律 + 红队自检 |
| `ascend-v2` | `/ascend-v2 任务` | 可验证版：验证卡（假设/基线/指标/阈值）+ 采纳记录 + 触发测试集 |
| `ascend-v3` | `/ascend-v3 任务` | 闸门版：按复杂度分档（放行/精简/完整）+ 记忆预填 + 可粘贴的升维记录 |

## 安装

```bash
git clone https://github.com/youyouhe/ascend-skills.git
cp -r ascend-skills/skills/* ~/.claude/skills/
```

重启 Claude Code 会话后生效。`ascend-v1/v2/v3` 为手动触发（`disable-model-invocation: true`）。

## 说明

- `ascend-v3` 的「记忆预填」读取 `~/.claude/projects/<project>/memory/MEMORY.md`，路径按你的环境调整；没有记忆文件时会写"无相关前科"。
- `ascend-v2` 首次使用时会在其 skill 目录创建 `adoption-log.md`。

## License

MIT
