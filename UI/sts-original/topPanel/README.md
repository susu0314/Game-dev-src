# 界面与交互组件 / topPanel

来源：用户上传的原版《Slay the Spire》资源；本次保持源文件内容与命名，核查日期 2026-10-03。

- 源提交：`cac427576f3517e8c9609a7f9e4a0ae5814b52ee`
- 本组文件：67
- 状态：源Git blob一致；图片/文本已检查；Unity尚未导入运行。音效尚未试听。
- 来源与接入范围见本批总说明。

## 文件与用途

| 文件 | 实际规格 | 字节数 | 用途/配套关系 |
|---|---|---:|---|
| [bar.png](bar.png) | 1920×128 P | 13006 | 顶部状态栏；用Unity组件绑定对应行为 |
| [blue/1.png](blue/1.png) | 128×128 P | 3909 | 能量球/顶部状态分层 1；单层不能代表完整效果 |
| [blue/1d.png](blue/1d.png) | 128×128 P | 3041 | 能量球/顶部状态分层 1d；单层不能代表完整效果 |
| [blue/2.png](blue/2.png) | 128×128 P | 6035 | 能量球/顶部状态分层 2；单层不能代表完整效果 |
| [blue/2d.png](blue/2d.png) | 128×128 P | 4860 | 能量球/顶部状态分层 2d；单层不能代表完整效果 |
| [blue/3.png](blue/3.png) | 128×128 P | 3737 | 能量球/顶部状态分层 3；单层不能代表完整效果 |
| [blue/3d.png](blue/3d.png) | 128×128 P | 2849 | 能量球/顶部状态分层 3d；单层不能代表完整效果 |
| [blue/4.png](blue/4.png) | 128×128 P | 4749 | 能量球/顶部状态分层 4；单层不能代表完整效果 |
| [blue/4d.png](blue/4d.png) | 128×128 P | 3942 | 能量球/顶部状态分层 4d；单层不能代表完整效果 |
| [blue/5.png](blue/5.png) | 128×128 RGBA | 5925 | 能量球/顶部状态分层 5；单层不能代表完整效果 |
| [blue/5d.png](blue/5d.png) | 128×128 P | 2660 | 能量球/顶部状态分层 5d；单层不能代表完整效果 |
| [blue/border.png](blue/border.png) | 128×128 P | 3920 | 能量球/顶部状态分层 border；单层不能代表完整效果 |
| [buttonL.png](buttonL.png) | 512×512 P | 8568 | 功能UI部件 topPanel/buttonL.png；保留原命名方便匹配 |
| [buttonLRed.png](buttonLRed.png) | 512×512 P | 8653 | 功能UI部件 topPanel/buttonLRed.png；保留原命名方便匹配 |
| [cancelButton.png](cancelButton.png) | 512×256 P | 3657 | 功能UI部件 topPanel/cancelButton.png；保留原命名方便匹配 |
| [cancelButtonOutline.png](cancelButtonOutline.png) | 512×256 P | 1413 | 功能UI部件 topPanel/cancelButtonOutline.png；保留原命名方便匹配 |
| [cancelButtonShadow.png](cancelButtonShadow.png) | 512×256 P | 1141 | 功能UI部件 topPanel/cancelButtonShadow.png；保留原命名方便匹配 |
| [confirmButton.png](confirmButton.png) | 512×256 P | 5108 | 功能UI部件 topPanel/confirmButton.png；保留原命名方便匹配 |
| [confirmButtonOutline.png](confirmButtonOutline.png) | 512×256 P | 1297 | 功能UI部件 topPanel/confirmButtonOutline.png；保留原命名方便匹配 |
| [confirmButtonShadow.png](confirmButtonShadow.png) | 512×256 P | 1054 | 功能UI部件 topPanel/confirmButtonShadow.png；保留原命名方便匹配 |
| [countCircle.png](countCircle.png) | 128×128 P | 1001 | 功能UI部件 topPanel/countCircle.png；保留原命名方便匹配 |
| [deck.png](deck.png) | 64×64 P | 2873 | 功能UI部件 topPanel/deck.png；保留原命名方便匹配 |
| [endTurnButton.png](endTurnButton.png) | 256×256 P | 8339 | 结束回合按钮；用Unity组件绑定对应行为 |
| [endTurnButtonGlow.png](endTurnButtonGlow.png) | 256×256 P | 11811 | 结束回合高亮；用Unity组件绑定对应行为 |
| [endTurnHover.png](endTurnHover.png) | 256×256 P | 7065 | 结束回合悬停态；用Unity组件绑定对应行为 |
| [energyBlueVFX.png](energyBlueVFX.png) | 256×256 P | 11511 | UI效果层 energyBlueVFX；需要游戏控制透明度/时间 |
| [energyGreenVFX.png](energyGreenVFX.png) | 256×256 P | 11311 | UI效果层 energyGreenVFX；需要游戏控制透明度/时间 |
| [energyPurpleVFX.png](energyPurpleVFX.png) | 256×256 P | 10211 | UI效果层 energyPurpleVFX；需要游戏控制透明度/时间 |
| [energyRedVFX.png](energyRedVFX.png) | 256×256 P | 11225 | UI效果层 energyRedVFX；需要游戏控制透明度/时间 |
| [floor.png](floor.png) | 64×64 P | 1555 | 楼层图标；用Unity组件绑定对应行为 |
| [gold.png](gold.png) | 64×64 P | 1770 | 金币图标；用Unity组件绑定对应行为 |
| [green/layer1.png](green/layer1.png) | 128×128 P | 1883 | 能量球/顶部状态分层 layer1；单层不能代表完整效果 |
| [green/layer1d.png](green/layer1d.png) | 128×128 P | 1648 | 能量球/顶部状态分层 layer1d；单层不能代表完整效果 |
| [green/layer2.png](green/layer2.png) | 128×128 P | 2760 | 能量球/顶部状态分层 layer2；单层不能代表完整效果 |
| [green/layer2d.png](green/layer2d.png) | 128×128 P | 2292 | 能量球/顶部状态分层 layer2d；单层不能代表完整效果 |
| [green/layer3.png](green/layer3.png) | 128×128 P | 3758 | 能量球/顶部状态分层 layer3；单层不能代表完整效果 |
| [green/layer3d.png](green/layer3d.png) | 128×128 P | 3159 | 能量球/顶部状态分层 layer3d；单层不能代表完整效果 |
| [green/layer4.png](green/layer4.png) | 128×128 P | 2507 | 能量球/顶部状态分层 layer4；单层不能代表完整效果 |
| [green/layer4d.png](green/layer4d.png) | 128×128 P | 2173 | 能量球/顶部状态分层 layer4d；单层不能代表完整效果 |
| [green/layer5.png](green/layer5.png) | 128×128 P | 4442 | 能量球/顶部状态分层 layer5；单层不能代表完整效果 |
| [green/layer5d.png](green/layer5d.png) | 128×128 P | 4041 | 能量球/顶部状态分层 layer5d；单层不能代表完整效果 |
| [green/layer6.png](green/layer6.png) | 256×256 P | 6008 | 能量球/顶部状态分层 layer6；单层不能代表完整效果 |
| [map.png](map.png) | 64×64 P | 2559 | 地图入口；用Unity组件绑定对应行为 |
| [panelGoldBag.png](panelGoldBag.png) | 64×64 RGBA | 3929 | 金币袋图标；用Unity组件绑定对应行为 |
| [panelHeart.png](panelHeart.png) | 64×64 RGBA | 2934 | 生命值图标；用Unity组件绑定对应行为 |
| [panel_heart_white.png](panel_heart_white.png) | 64×64 P | 700 | 功能UI部件 topPanel/panel_heart_white.png；保留原命名方便匹配 |
| [peek_button.png](peek_button.png) | 128×128 P | 7147 | 功能UI部件 topPanel/peek_button.png；保留原命名方便匹配 |
| [proceedButton.png](proceedButton.png) | 512×512 P | 9680 | 继续按钮；用Unity组件绑定对应行为 |
| [proceedButtonOutline.png](proceedButtonOutline.png) | 512×512 P | 2623 | 功能UI部件 topPanel/proceedButtonOutline.png；保留原命名方便匹配 |
| [proceedButtonShadow.png](proceedButtonShadow.png) | 512×512 P | 2184 | 功能UI部件 topPanel/proceedButtonShadow.png；保留原命名方便匹配 |
| [purple/border.png](purple/border.png) | 128×128 P | 4670 | 能量球/顶部状态分层 border；单层不能代表完整效果 |
| [purple/l1.png](purple/l1.png) | 128×128 P | 5733 | 能量球/顶部状态分层 l1；单层不能代表完整效果 |
| [purple/l2.png](purple/l2.png) | 128×128 P | 1057 | 能量球/顶部状态分层 l2；单层不能代表完整效果 |
| [purple/l3.png](purple/l3.png) | 128×128 P | 3230 | 能量球/顶部状态分层 l3；单层不能代表完整效果 |
| [purple/l4.png](purple/l4.png) | 128×128 P | 2249 | 能量球/顶部状态分层 l4；单层不能代表完整效果 |
| [red/layer1.png](red/layer1.png) | 128×128 P | 4134 | 能量球/顶部状态分层 layer1；单层不能代表完整效果 |
| [red/layer1d.png](red/layer1d.png) | 128×128 P | 3335 | 能量球/顶部状态分层 layer1d；单层不能代表完整效果 |
| [red/layer2.png](red/layer2.png) | 128×128 P | 6038 | 能量球/顶部状态分层 layer2；单层不能代表完整效果 |
| [red/layer2d.png](red/layer2d.png) | 128×128 P | 4836 | 能量球/顶部状态分层 layer2d；单层不能代表完整效果 |
| [red/layer3.png](red/layer3.png) | 128×128 P | 5036 | 能量球/顶部状态分层 layer3；单层不能代表完整效果 |
| [red/layer3d.png](red/layer3d.png) | 128×128 P | 4342 | 能量球/顶部状态分层 layer3d；单层不能代表完整效果 |
| [red/layer4.png](red/layer4.png) | 128×128 P | 5107 | 能量球/顶部状态分层 layer4；单层不能代表完整效果 |
| [red/layer4d.png](red/layer4d.png) | 128×128 P | 4148 | 能量球/顶部状态分层 layer4d；单层不能代表完整效果 |
| [red/layer5.png](red/layer5.png) | 128×128 P | 2948 | 能量球/顶部状态分层 layer5；单层不能代表完整效果 |
| [red/layer5d.png](red/layer5d.png) | 128×128 P | 2344 | 能量球/顶部状态分层 layer5d；单层不能代表完整效果 |
| [red/layer6.png](red/layer6.png) | 128×128 P | 5189 | 能量球/顶部状态分层 layer6；单层不能代表完整效果 |
| [settings.png](settings.png) | 64×64 P | 3153 | 功能UI部件 topPanel/settings.png；保留原命名方便匹配 |

原路径、哈希与取舍理由可在 [迁移清单](../../../Collections/sts-original/manifest.json) 找到。
