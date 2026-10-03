# 用户上传原版素材 · 筛选整理

来源：用户上传的“杀戮尖塔全套素材包”，源提交 `cac427576f3517e8c9609a7f9e4a0ae5814b52ee`。整理日期：2026-10-03。按用户个人学习、非商用原型要求整理；这些是原游戏资源，没有改标为 CC0、MIT 或统一开源许可。

**2614个源文件全部有去向：905个保留，1709个放入废弃目录。** 成套角色/敌人骨骼优先保留；其他类目按原型价值筛选。源包原来已是展开目录，本次按用途分类迁移。

## 分类入口

| 分类 | 文件数 | MiB |
|---|---:|---:|
| [废弃/暂不采用](../../Discarded/sts-original/README.md) | 1709 | 198.83 |
| [交互与元素音效](../../Audio/sts-original/README.md) | 72 | 4.02 |
| [事件与场景背景](../../EventBackgrounds/sts-original/README.md) | 29 | 7.12 |
| [卡牌框与卡牌UI](../../CardFrames/sts-original/README.md) | 18 | 2.99 |
| [卡牌插画候选](../../CardArt/sts-original/README.md) | 27 | 1.04 |
| [人物与NPC](../../Characters/sts-original/README.md) | 46 | 3.80 |
| [遗物与器具](../../Relics/sts-original/README.md) | 75 | 0.22 |
| [敌人与Boss](../../Enemies/sts-original/README.md) | 215 | 9.60 |
| [界面与交互组件](../../UI/sts-original/README.md) | 236 | 2.50 |
| [特效与能量球](../../VFX/sts-original/README.md) | 49 | 3.68 |
| [药水分层](../../Potions/sts-original/README.md) | 88 | 0.12 |
| [路线地图](../../Maps/sts-original/README.md) | 50 | 1.53 |

## 重要实际情况

- 没有发现 FBX/OBJ/GLB 等3D模型；人物和多数敌人是2D Spine。共73套骨骼：72套3.4.02、1套3.4.01。65份位于敌人目录，5份为玩家角色（含观者眼部）、3份NPC/特殊角色。以迁移清单中的实际JSON为准。
- JSON可以解析；所有atlas图片页存在，附件名称均能对应到图集区域；905个保留文件均校对源Git blob。687张PNG/JPG已解码检查；详见[验证记录](validation.json)。
- 动作名称逐组记录。有的只有`idle`或`animation`，不能称作完整攻击/移动/死亡动画库。
- PNG/JPG按原文件解码检查；72个音效记录声道/采样率/时长，尚未试听。大图表缺少配套坐标的保持原图，不进行猜测切片。
- 未打开Unity、未安装运行时、未修改项目或生成`.meta`/预制体。Spine3.4数据不能凭文件齐全就宣布兼容当前Unity。

## 建议先取用

1. 四职业角色骨骼与角色选择插画；优先用静态角色图建立战斗占位，再单独验证骨骼导入。
2. 敌人中先选史莱姆、机械哨兵、球形/元素类等少量候选，避免为用齐所有敌人扩大卡池。
3. 结束回合、敌人意图、抽/弃牌堆、事件/奖励框和分支地图节点；这些同类游戏专用组件比普通按钮更难替换。
4. 雷电/冰霜能量球、水滴、火焰、瓶装雷电/龙卷风与相关卡面，补充气象主题。

玩法/气象用途是本项目的建议，不能将原版职业、遗物或图片误写成真实气象仪器与科学示意。

- [迁移清单与逐文件验证](manifest.json)：原路径→新路径、保留/废弃理由、源Git blob、选用文件SHA256与规格。
- [骨骼与Unity交接](IntegrationNotes.md)
- [预览图](../../Previews/sts-original/cards.jpg)
- [废弃文件入口](../../Discarded/sts-original/README.md)

本批没有制作Game Development Studio canonical package，当前环境没有`game-dev`；整理与Git blob校验不等于`package verify`或Unity运行验收。
