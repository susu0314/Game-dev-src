# 界面与交互组件 / intent

来源：用户上传的原版《Slay the Spire》资源；本次保持源文件内容与命名，核查日期 2026-10-03。

- 源提交：`cac427576f3517e8c9609a7f9e4a0ae5814b52ee`
- 本组文件：46
- 状态：源Git blob一致；图片/文本已检查；Unity尚未导入运行。音效尚未试听。
- 来源与接入范围见本批总说明。

## 文件与用途

| 文件 | 实际规格 | 字节数 | 用途/配套关系 |
|---|---|---:|---|
| [attack/attack_intent_1.png](attack/attack_intent_1.png) | 128×128 P | 2114 | 攻击强度等级 1 的敌人意图图标 |
| [attack/attack_intent_2.png](attack/attack_intent_2.png) | 128×128 P | 2398 | 攻击强度等级 2 的敌人意图图标 |
| [attack/attack_intent_3.png](attack/attack_intent_3.png) | 128×128 P | 2682 | 攻击强度等级 3 的敌人意图图标 |
| [attack/attack_intent_4.png](attack/attack_intent_4.png) | 128×128 P | 3062 | 攻击强度等级 4 的敌人意图图标 |
| [attack/attack_intent_5.png](attack/attack_intent_5.png) | 128×128 P | 3022 | 攻击强度等级 5 的敌人意图图标 |
| [attack/attack_intent_6.png](attack/attack_intent_6.png) | 128×128 P | 3762 | 攻击强度等级 6 的敌人意图图标 |
| [attack/attack_intent_7.png](attack/attack_intent_7.png) | 128×128 P | 3430 | 攻击强度等级 7 的敌人意图图标 |
| [attackBuff.png](attackBuff.png) | 64×64 P | 2655 | 攻击并增益意图；用Unity组件绑定对应行为 |
| [attackDebuff.png](attackDebuff.png) | 64×64 P | 2829 | 攻击并减益意图；用Unity组件绑定对应行为 |
| [attackDefend.png](attackDefend.png) | 64×64 P | 2497 | 攻击并防御意图；用Unity组件绑定对应行为 |
| [buff1.png](buff1.png) | 64×64 P | 2667 | 功能UI部件 intent/buff1.png；保留原命名方便匹配 |
| [buff1L.png](buff1L.png) | 128×128 P | 3004 | 功能UI部件 intent/buff1L.png；保留原命名方便匹配 |
| [buffVFX1.png](buffVFX1.png) | 32×32 P | 1012 | UI效果层 buffVFX1；需要游戏控制透明度/时间 |
| [buffVFX2.png](buffVFX2.png) | 32×32 P | 1105 | UI效果层 buffVFX2；需要游戏控制透明度/时间 |
| [buffVFX3.png](buffVFX3.png) | 32×32 P | 931 | UI效果层 buffVFX3；需要游戏控制透明度/时间 |
| [debuff1.png](debuff1.png) | 64×64 P | 3149 | 功能UI部件 intent/debuff1.png；保留原命名方便匹配 |
| [debuff1L.png](debuff1L.png) | 128×128 P | 3234 | 功能UI部件 intent/debuff1L.png；保留原命名方便匹配 |
| [debuff2.png](debuff2.png) | 64×64 P | 3974 | 功能UI部件 intent/debuff2.png；保留原命名方便匹配 |
| [debuff2L.png](debuff2L.png) | 128×128 P | 4117 | 功能UI部件 intent/debuff2L.png；保留原命名方便匹配 |
| [debuffVFX1.png](debuffVFX1.png) | 32×32 P | 1193 | UI效果层 debuffVFX1；需要游戏控制透明度/时间 |
| [debuffVFX2.png](debuffVFX2.png) | 32×32 P | 732 | UI效果层 debuffVFX2；需要游戏控制透明度/时间 |
| [debuffVFX3.png](debuffVFX3.png) | 32×32 P | 808 | UI效果层 debuffVFX3；需要游戏控制透明度/时间 |
| [defend.png](defend.png) | 64×64 P | 2427 | 防御意图；用Unity组件绑定对应行为 |
| [defendBuff.png](defendBuff.png) | 64×64 P | 3223 | 功能UI部件 intent/defendBuff.png；保留原命名方便匹配 |
| [defendBuffL.png](defendBuffL.png) | 128×128 P | 3345 | 功能UI部件 intent/defendBuffL.png；保留原命名方便匹配 |
| [defendL.png](defendL.png) | 128×128 P | 2466 | 功能UI部件 intent/defendL.png；保留原命名方便匹配 |
| [escape.png](escape.png) | 64×64 P | 2095 | 逃跑意图；用Unity组件绑定对应行为 |
| [escapeL.png](escapeL.png) | 128×128 P | 2129 | 功能UI部件 intent/escapeL.png；保留原命名方便匹配 |
| [magic.png](magic.png) | 64×64 P | 3028 | 魔法意图；用Unity组件绑定对应行为 |
| [magicL.png](magicL.png) | 128×128 P | 3149 | 功能UI部件 intent/magicL.png；保留原命名方便匹配 |
| [placeholder.png](placeholder.png) | 64×64 P | 2914 | 功能UI部件 intent/placeholder.png；保留原命名方便匹配 |
| [sleep.png](sleep.png) | 64×64 P | 2785 | 睡眠意图图标；用Unity组件绑定对应行为 |
| [sleepL.png](sleepL.png) | 128×128 P | 2916 | 功能UI部件 intent/sleepL.png；保留原命名方便匹配 |
| [special.png](special.png) | 64×64 P | 1668 | 特殊动作意图；用Unity组件绑定对应行为 |
| [specialL.png](specialL.png) | 128×128 P | 1707 | 功能UI部件 intent/specialL.png；保留原命名方便匹配 |
| [stun.png](stun.png) | 64×64 P | 1818 | 眩晕意图；用Unity组件绑定对应行为 |
| [stunL.png](stunL.png) | 128×128 P | 1841 | 功能UI部件 intent/stunL.png；保留原命名方便匹配 |
| [tip/1.png](tip/1.png) | 64×64 P | 2768 | 能量球/顶部状态分层 1；单层不能代表完整效果 |
| [tip/2.png](tip/2.png) | 64×64 P | 2842 | 能量球/顶部状态分层 2；单层不能代表完整效果 |
| [tip/3.png](tip/3.png) | 64×64 P | 2806 | 能量球/顶部状态分层 3；单层不能代表完整效果 |
| [tip/4.png](tip/4.png) | 64×64 P | 2935 | 能量球/顶部状态分层 4；单层不能代表完整效果 |
| [tip/5.png](tip/5.png) | 64×64 P | 2936 | 能量球/顶部状态分层 5；单层不能代表完整效果 |
| [tip/6.png](tip/6.png) | 64×64 P | 3281 | 能量球/顶部状态分层 6；单层不能代表完整效果 |
| [tip/7.png](tip/7.png) | 64×64 P | 3071 | 功能UI部件 intent/tip/7.png；保留原命名方便匹配 |
| [unknown.png](unknown.png) | 64×64 RGBA | 3094 | 未知意图；用Unity组件绑定对应行为 |
| [unknownL.png](unknownL.png) | 128×128 P | 1230 | 功能UI部件 intent/unknownL.png；保留原命名方便匹配 |

原路径、哈希与取舍理由可在 [迁移清单](../../../Collections/sts-original/manifest.json) 找到。
