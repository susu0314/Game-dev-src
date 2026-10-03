# 敌人与Boss / theForest/awakenedOne

来源：用户上传的原版《Slay the Spire》资源；本次保持源文件内容与命名，核查日期 2026-10-03。

- 源提交：`cac427576f3517e8c9609a7f9e4a0ae5814b52ee`
- 本组文件：3
- 状态：源Git blob一致；图片/文本已检查；Unity尚未导入运行。音效尚未试听。
- 来源与接入范围见本批总说明。

## 骨骼组 skeleton.json

Spine 3.4.02；48 骨骼；16 槽位。实际动作：`Attack_1`, `Attack_2`, `Hit`, `Idle_1`, `Idle_2`。图集图片页：AwakenedOne.png。

已核对图片页、附件区域名称均存在。动作仅以JSON实际内容为准；不因保留整套资源而声称具备攻击/移动/死亡等所有动作。保持JSON、atlas和贴图同目录及其大小写文件名。

## 文件与用途

| 文件 | 实际规格 | 字节数 | 用途/配套关系 |
|---|---|---:|---|
| [AwakenedOne.png](AwakenedOne.png) | 1024×256 RGBA | 132547 | 骨骼图集贴图；不是完整角色独立立绘 |
| [skeleton.atlas](skeleton.atlas) | 图集索引；图片页 AwakenedOne.png | 1688 | 图片页、区域与旋转/裁切索引；不可与贴图分离 |
| [skeleton.json](skeleton.json) | Spine 3.4.02 / 48骨骼 / 16槽位 | 186462 | 骨骼与动作数据；和同目录atlas及其图片页一起使用 |

原路径、哈希与取舍理由可在 [迁移清单](../../../../Collections/sts-original/manifest.json) 找到。
