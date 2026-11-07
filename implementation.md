# 实现与复现索引

| 待归档源码包 | 关联工作 | 核对入口 |
| --- | --- | --- |
| `robottt.zip` | GR00T / RoboTTT 的 DiT 和 Fast Weights 适配，Stage-1 训练及 Stage-2 诊断 | Action Head、TTT 内层更新、FP32/BF16 边界、Prefix mask、分段截断、训练配置和评估脚本 |
| `smolvla-robottt.zip` | SmolVLA 小模型上的 RoboTTT 适配 | TTT 插入位置、观察输入、采集台 human-video 模式和训练入口。项目记录中小模型版本已接通，训练待完成 |
| `Zero-WAM.zip` | SO-101 配对数据、Token Packing、后训练和部署 | 配对数据 schema、训练配置、视频与动作输入、WebSocket 服务与客户端、关节增量转换、评测与解码入口 |

DemoDiffusion 的记录还涉及 SmolVLA 采样器与 π0.5 / LIBERO-90 仿真评测。该实现是否随上述源码包提供，需要查阅归档清单后确认。

收到源码后，按上游来源和许可证整理保留的实现，再将以下信息补到每条路线：

1. 上游版本或 commit，以及本人新增或适配的文件和函数。
2. 模型权重、依赖、数据结构、任务及布局划分、配置和训练入口。
3. 离线评测命令、输入示例、输出字段与结果来源。
4. Zero-WAM 的部署入口、协议字段、模型与机器人运行环境，以及演示对应的 checkpoint。

本索引记录了待核对的范围。训练与部署命令需要依据实际入口、依赖和权重版本补全。
