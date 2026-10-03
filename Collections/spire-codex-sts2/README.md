# Spire Codex · 杀戮尖塔2二维素材补充

来源：[用户提供的图片目录](https://spire-codex.com/zhs/images)，主版本 **v0.107.1**，核查日期2026-10-03。本轮下载 **433项来源**，分为10类：**429张静态图、4个预渲染动作**。提供 **435张PNG** 与动作逐帧坐标/时长，同时用ZIP保留所有选用WebP的原文件内容。

## 分类入口

| 分类 | 选用来源数 |
|---|---:|
| [二维人物](../../Characters/spire-codex-sts2/README.md) | 7 |
| [二维敌人与Boss](../../Enemies/spire-codex-sts2/README.md) | 112 |
| [气象/元素卡牌插画](../../CardArt/spire-codex-sts2/README.md) | 20 |
| [功能UI与状态图标](../../UI/spire-codex-sts2/README.md) | 125 |
| [卡框与费用标记](../../CardFrames/spire-codex-sts2/README.md) | 60 |
| [路线地图节点](../../Maps/spire-codex-sts2/README.md) | 25 |
| [气象与战斗特效贴图](../../VFX/spire-codex-sts2/README.md) | 49 |
| [环境背景](../../EventBackgrounds/spire-codex-sts2/README.md) | 5 |
| [成品药水](../../Potions/spire-codex-sts2/README.md) | 16 |
| [遗物与器具](../../Relics/spire-codex-sts2/README.md) | 14 |

## 取用顺序与范围

1. 完整二维角色和敌人PNG可直接建立战斗画面，优先取用少量符合项目风格的候选。
2. 卡框、费用底图、结束回合、抽/弃/消耗牌堆、敌人意图、血条和奖励按钮组合成自己的卡牌UI。
3. 使用无文字卡牌原插画，卡牌名称、描述与效果由本项目定义。没有整体搬入多语言整卡或大量附魔组合图。
4. 雷电、云雾、水流、冰霜球、烟尘与遮罩作为天气VFX部件；原图内flipbook没有配套时序/网格证据时保留整图待切片。

这些资源包含原游戏导出图，以及网站基于原骨骼渲染的静态/动作图。网站的格式处理、烟雾占位替换等不等同于游戏编辑工程原件。本轮获取的是图片，不含Spine编辑工程或游戏模型/行为脚本。

## 格式与核查

WebP经解码转换为RGBA PNG，保留下载文件的解码像素、原尺寸和透明度；不声称恢复站点处理前的像素。所选动作完整转帧，保留每帧duration_ms，按最长2048像素分成图表页，每页与源帧的像素哈希对应。

所有原下载文件均记录URL、响应ETag/Last-Modified、字节数与SHA256；源文件ZIP按成员复核；PNG重读并逐像素比对。版本来自发布目录，不将主版本与Beta资产混写。

本次为素材仓库整理，未导入Unity、未生成.meta/场景/预制体，也未进行运行时或视觉玩法验收。Game Development Studio canonical package/admission不在本轮交付范围。

## 来源标注

按用户个人学习、非商用原型要求整理。站点服务免费可访问，但[服务条款](https://spire-codex.com/zhs/terms)注明游戏美术归Mega Crit所有；[网站代码许可](https://github.com/ptrlrd/spire-codex/blob/main/LICENSE.md)是PolyForm Noncommercial，与游戏美术分别记录。这批文件不标成CC0/MIT。

## 查询与接入

- [Unity图片/图表接入说明](IntegrationNotes.md)
- [逐项来源、输出、哈希与取舍清单](manifest.json)
- [验证记录](validation.json)
- [原下载文件ZIP](../../Sources/spire-codex-sts2/README.md)
- [未选用远程项索引](../../Discarded/spire-codex-sts2/README.md)

完整下载目录计数（用于判断筛选范围，以下文件没有整体下载）：

| 站点类别 | 文件数 | 本轮规则 |
|---|---:|---|
| cards | 17239 | 跳过多语言与组合整卡批量库 |
| assets | 5998 | 选择具明确用途的二维成品/部件，详见清单 |
| monsters | 116 | 选择具明确用途的二维成品/部件，详见清单 |
| monsters-skins | 68 | 选择具明确用途的二维成品/部件，详见清单 |
| relics | 335 | 选择具明确用途的二维成品/部件，详见清单 |
| potions | 65 | 选择具明确用途的二维成品/部件，详见清单 |
| backgrounds | 25 | 选择具明确用途的二维成品/部件，详见清单 |
| card-frames | 98 | 选择具明确用途的二维成品/部件，详见清单 |
| characters | 5 | 选择具明确用途的二维成品/部件，详见清单 |
| enchantments | 24 | 选择具明确用途的二维成品/部件，详见清单 |
| afflictions-cards | 167250 | 跳过多语言与组合整卡批量库 |
| enchantments-cards | 401400 | 跳过多语言与组合整卡批量库 |
| animations | 1808 | 选择具明确用途的二维成品/部件，详见清单 |

本批独立于首批气象开源资源和用户上传的一代原版素材，三个来源分别记录。
