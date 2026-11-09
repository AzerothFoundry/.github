# AzerothFoundry

**让 AI Bot 持续生活，让人类自由参与。**

*An AI-inhabited Azeroth, open to human players.*

我们希望在 WoW 1.12.1 的世界里，构建一个由 AI Bot 持续参与的生态：角色拥有持续的身份和成长，在野外冒险、城镇生活、结伴战斗，也与其他角色竞争和合作。人类可以进入这个世界，和 Bot 组队、交易、切磋，参与世界中正在发生的活动。

这是我们的方向。当前公开版本以**服务端规则、状态机和场景协作**驱动 Bot，正在逐步补齐长期活动、行为记录与扩展接口；尚未接入大模型或强化学习，也不代表所有世界活动都已经自治运行。

## 从哪里开始

**[realm：项目总入口、部署进度与版本组合](https://github.com/AzerothFoundry/realm)**

| 项目 | 职责 |
| --- | --- |
| [vmangos-core](https://github.com/AzerothFoundry/vmangos-core/tree/feat/realm-integration) | 服务端、持久世界 Bot、组队与战场行为 |
| [realm-admin](https://github.com/AzerothFoundry/realm-admin) | 容器化账号管理与服务器参数管理 |
| [addons](https://github.com/AzerothFoundry/addons) | 游戏内操作界面、自研便利插件和第三方插件清单 |
| [benilla](https://github.com/AzerothFoundry/benilla/tree/feat/realm-client-compat) | 以标准 1.12.1 兼容为目标的客户端 fork |
| [AutoQuest](https://github.com/AzerothFoundry/AutoQuest/tree/feat/vanilla-compat-options) | 自动交接任务插件的兼容与选项修复 |

目前发布的是源码候选，镜像、完整体验包和全新环境部署验收仍在推进；请以 realm 的版本清单和交付清单为准。

## 我们坚持的边界

- **世界智能在服务端。** Bot 特性不要求修改客户端代码，客户端继续兼容其他标准 1.12.1 服务端。
- **插件能够降级。** 服务器不支持扩展时友好提示，不报错或刷屏；现有历史改动仍需按此标准逐项验收。
- **行为可解释、可验证。** 逐步建立观察、决策、执行和结果记录，再探索外部模型与学习策略。
- **尊重上游。** 通用修复拆成小 PR，定制玩法留在 fork；保留来源与各项目许可证。

欢迎从复现问题、改进策略、设计活动、补充测试或完善部署文档开始。游戏素材由使用者自行提供，本组织不分发游戏资源。
