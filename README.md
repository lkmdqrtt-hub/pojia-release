# 网络小白一键破甲

把电脑上 15 个 AI 客户端「自己改不到的内置提示词」，换成你自己写的一份。

> **本软件永久免费，不通过任何渠道销售。**
> **任何向你收费出售本软件的行为均为诈骗。**

---

## 这是什么

很多 AI 客户端（Codex CLI、Cursor、Claude Code、Gemini CLI……）都有一份内置的
系统提示词，用户改不到。这个工具做的事很简单：

1. 找到每个客户端存提示词的文件
2. 把你自己的人格文本写进去
3. 想恢复时一键还原成官方原版

只读写本地文件，不需要账号，不上传任何东西。

## 支持的客户端

| 客户端 | 注入位置 |
|---|---|
| DeepSeek Harness | 三层文件补丁 |
| WorkBuddy | 六层靶点 + 云记忆 |
| ZCode（智谱） | AGENTS.md + Memory + 系统提示词 |
| OpenAI Codex CLI | `config.toml` 的 `model_instructions_file` |
| Cursor | `rules/pojia-inject.mdc` |
| Claude Code | `CLAUDE.md`（用户级） |
| Gemini CLI | `GEMINI.md` |
| Qwen Code | `QWEN.md` |
| iFlow CLI | `IFLOW.md` |
| Trae | `rules/project_rules.md` |
| CodeBuddy | `CODEBUDDY.md` |
| OpenCode | `AGENTS.md` |
| Windsurf | `memories/global_rules.md` |
| Cline | `pojie-inject.md` |
| GitHub Copilot CLI | `copilot-instructions.md` |

## 两个版本

| 版本 | 人格来源 | 适合谁 |
|---|---|---|
| 离线版 | exe 同目录的 `persona.md`，自己改 | 不想联网、想自己完全掌控 |
| 网络版 | 云端下发，作者统一维护 | 不想折腾，跟着更新走 |

两个版本功能一致，只是人格从哪来不同。

## 界面

单窗口，左侧三个导航：

- **检测**：列出 15 个客户端，显示装没装、补没补
- **操作**：破甲 / 还原 / 刷新
- **日志**：实时滚动，能看到每一步做了什么

不需要点也能看到全部状态。

## 获取方式

**不在这里下载。** 本仓库只放说明文字，不放安装包。

本软件不公开发布，仅由作者私下分享给朋友。如果你是从其他渠道拿到的，
那都不是官方版本——官方版本永远免费，任何收费行为都是诈骗。

## 免费声明

本软件永久免费，不通过任何渠道销售。

如果你是通过付费渠道拿到的：

1. 立即停止付款
2. 向支付平台申诉
3. 到官方渠道获取免费版本

收费卖这个软件的人，卖的不是软件，是信息差。

## 免责

本软件按「现状」提供，不附带任何明示或暗示的担保。

使用本软件会修改你电脑上其他软件的配置文件，可能导致：

- 客户端行为异常
- 账号被平台判定异常
- 配置丢失

上述风险由使用者自行承担。软件内置完整还原功能，出问题可以一键恢复。

**请在使用前确认你拥有所修改软件的合法使用权。**

## 致谢

本项目基于 [pojia-next](https://github.com/z91772524-ai/pojia-next) 二次修改。

原作者：**z91772524-ai**

原项目采用 MIT 许可，允许使用、修改、分发与商业使用。
本版本同样以 MIT 许可发布，完整版权声明见 [LICENSE](LICENSE)。

原项目地址：https://github.com/z91772524-ai/pojia-next

## 许可

MIT License。允许自由使用、修改、分发。

分发时必须保留 `LICENSE` 中的原始版权声明。
