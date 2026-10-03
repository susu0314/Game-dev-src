# card-trail-godot · VFX

来源：fragule-hub/learning_ss2-card_trail_vfx。上游代码 MIT；场景引用的 pimen big/small 贴图未复制，原代码和参数作为静态参考。

本目录 10 个原文件/解包文件，0 个配套透明PNG。用途为本仓库的原型建议；无三维模型。

本批未收录两个第三方粒子贴图、project.godot 与引擎导入缓存。原场景依赖仍指向 res://assets/big.png 和 small.png，因此这是一份代码/参数参考，尚不是可运行Godot工程或Unity特效预制体。

[查看参数与Unity移植说明](../../Collections/community-supplement-2026-10/UnityNotes.md)。

| 文件 | 实测规格 | 内容与用途 | 来源/作者 |
|---|---|---|---|
| [LICENSE](LICENSE) | 文本 · 1,068 B | 上游 MIT 许可全文 | [来源](https://raw.githubusercontent.com/fragule-hub/learning_ss2-card_trail_vfx/2caedd8bcbf4a72f3b91c28ae11fb270c544d60a/LICENSE) |
| [UPSTREAM-README.md](UPSTREAM-README.md) | MD · 263 B | 上游来源和作者感谢，保留原内容 | [来源](https://raw.githubusercontent.com/fragule-hub/learning_ss2-card_trail_vfx/2caedd8bcbf4a72f3b91c28ae11fb270c544d60a/README.md) |
| [procedural_card_fly_vfx.gd](procedural_trail/procedural_card_fly_vfx.gd) | GD · 7,006 B | 二次贝塞尔飞行、前视旋转、加速与缩小；适合卡牌投射到目标的运动参考 | [来源](https://raw.githubusercontent.com/fragule-hub/learning_ss2-card_trail_vfx/2caedd8bcbf4a72f3b91c28ae11fb270c544d60a/procedural_trail/procedural_card_fly_vfx.gd) |
| [procedural_card_fly_vfx.tscn](procedural_trail/procedural_card_fly_vfx.tscn) | TSCN · 1,817 B | 飞行光形与脚本挂载关系；Godot 场景格式，不可直接导入 Unity | [来源](https://raw.githubusercontent.com/fragule-hub/learning_ss2-card_trail_vfx/2caedd8bcbf4a72f3b91c28ae11fb270c544d60a/procedural_trail/procedural_card_fly_vfx.tscn) |
| [procedural_card_trail.gd](procedural_trail/procedural_card_trail.gd) | GD · 3,402 B | 按寿命淘汰拖尾点、按移动距离补点和平滑曲线；适合移植成网格带或 TrailRenderer 行为参考 | [来源](https://raw.githubusercontent.com/fragule-hub/learning_ss2-card_trail_vfx/2caedd8bcbf4a72f3b91c28ae11fb270c544d60a/procedural_trail/procedural_card_trail.gd) |
| [procedural_card_trail_vfx.gd](procedural_trail/procedural_card_trail_vfx.gd) | GD · 3,453 B | 跟随主体、入场显现、淡出和停止粒子；适合整理特效生命周期 | [来源](https://raw.githubusercontent.com/fragule-hub/learning_ss2-card_trail_vfx/2caedd8bcbf4a72f3b91c28ae11fb270c544d60a/procedural_trail/procedural_card_trail_vfx.gd) |
| [procedural_card_trail_vfx.tscn](procedural_trail/procedural_card_trail_vfx.tscn) | TSCN · 6,253 B | 三层 Line2D、宽度曲线、颜色渐变和两组粒子参数；需替换缺失贴图 | [来源](https://raw.githubusercontent.com/fragule-hub/learning_ss2-card_trail_vfx/2caedd8bcbf4a72f3b91c28ae11fb270c544d60a/procedural_trail/procedural_card_trail_vfx.tscn) |
| [procedural_math_helper.gd](procedural_trail/procedural_math_helper.gd) | GD · 464 B | 二次贝塞尔曲线数学函数；可改写为 Unity Vector2/Vector3 计算 | [来源](https://raw.githubusercontent.com/fragule-hub/learning_ss2-card_trail_vfx/2caedd8bcbf4a72f3b91c28ae11fb270c544d60a/procedural_trail/procedural_math_helper.gd) |
| [procedural_trail_demo.gd](procedural_trail/procedural_trail_demo.gd) | GD · 6,767 B | 演示场景控制、输入和发射逻辑；作为调参交互参考 | [来源](https://raw.githubusercontent.com/fragule-hub/learning_ss2-card_trail_vfx/2caedd8bcbf4a72f3b91c28ae11fb270c544d60a/procedural_trail/procedural_trail_demo.gd) |
| [procedural_trail_demo.tscn](procedural_trail/procedural_trail_demo.tscn) | TSCN · 3,504 B | 演示场景节点结构及输入界面；不作为可运行完整工程交付 | [来源](https://raw.githubusercontent.com/fragule-hub/learning_ss2-card_trail_vfx/2caedd8bcbf4a72f3b91c28ae11fb270c544d60a/procedural_trail/procedural_trail_demo.tscn) |

[完整来源/哈希清单](../../Collections/community-supplement-2026-10/manifest.json) · [本批总览](../../Collections/community-supplement-2026-10/README.md)。未启动Unity、未验证导入、材质或运行效果。
