# 敌人与Boss / theCity/byrd

来源：用户上传的原版《Slay the Spire》资源；本次保持源文件内容与命名，核查日期 2026-10-03。

- 源提交：`cac427576f3517e8c9609a7f9e4a0ae5814b52ee`
- 本组文件：6
- 状态：源Git blob一致；图片/文本已检查；Unity尚未导入运行。音效尚未试听。
- 来源与接入范围见本批总说明。

## 骨骼组 flying.json

Spine 3.4.02；83 骨骼；15 槽位。实际动作：`idle_flap`。图集图片页：flying.png。

已核对图片页、附件区域名称均存在。动作仅以JSON实际内容为准；不因保留整套资源而声称具备攻击/移动/死亡等所有动作。保持JSON、atlas和贴图同目录及其大小写文件名。

## 骨骼组 grounded.json

Spine 3.4.02；41 骨骼；10 槽位。实际动作：`head_lift`, `idle`。图集图片页：grounded.png。

已核对图片页、附件区域名称均存在。动作仅以JSON实际内容为准；不因保留整套资源而声称具备攻击/移动/死亡等所有动作。保持JSON、atlas和贴图同目录及其大小写文件名。

## 文件与用途

| 文件 | 实际规格 | 字节数 | 用途/配套关系 |
|---|---|---:|---|
| [flying.atlas](flying.atlas) | 图集索引；图片页 flying.png | 994 | 图片页、区域与旋转/裁切索引；不可与贴图分离 |
| [flying.json](flying.json) | Spine 3.4.02 / 83骨骼 / 15槽位 | 92902 | 骨骼与动作数据；和同目录atlas及其图片页一起使用 |
| [flying.png](flying.png) | 512×128 RGBA | 45811 | 骨骼图集贴图；不是完整角色独立立绘 |
| [grounded.atlas](grounded.atlas) | 图集索引；图片页 grounded.png | 698 | 图片页、区域与旋转/裁切索引；不可与贴图分离 |
| [grounded.json](grounded.json) | Spine 3.4.02 / 41骨骼 / 10槽位 | 43901 | 骨骼与动作数据；和同目录atlas及其图片页一起使用 |
| [grounded.png](grounded.png) | 512×256 RGBA | 37356 | 骨骼图集贴图；不是完整角色独立立绘 |

原路径、哈希与取舍理由可在 [迁移清单](../../../../Collections/sts-original/manifest.json) 找到。
