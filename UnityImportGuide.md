# Unity 原型导入与选择建议

本次只完成素材采集与文件检查；未接入 Unity Editor。`unity_tested: false` 应保持到真实导入/运行验证后再改。

## 先选一条视觉路线

建议首轮使用清晰线条天气状态图标 + 简单卡框 + 云角色 + 少量天气特效。像素背景、古典金边框、现代细线图标是不同候选风格，不建议全部混用。图片调色只能改善颜色一致性，不能消除绘画风格差异。

| 内容 | 建议设置/操作 | 简单验收 |
|---|---|---|
| 单张卡框、药水、角色 PNG | Texture Type = Sprite (2D and UI)，Single；用 Image/SpriteRenderer 引用 | 检查透明边缘、裁切和小尺寸可读性 |
| 像素云、雪地瓦片 | Point 过滤；瓦片表需要 Multiple 并按实际网格切分 | 整数倍显示，避免模糊；确认切片范围 |
| Lucide SVG | 导出透明 PNG（建议 128 或 256 像素），明确 currentColor；再按普通 Sprite 导入 | 不要把 XML 文本直接赋给 Image；检验 24/32 像素显示 |
| 闪电球/雨滴独立帧 | 按末尾帧号数值排序，制作 Sprite 动画 | 闪电球 20 帧、雨滴 30 帧是否连续；帧率自行试听/试看调整 |
| 雾、烟雾、拖尾 | 基础贴图；用自己的材质/粒子组件控制透明度和运动 | 检查雾是否遮挡卡牌文字，雷击是否过亮 |
| 天空全景 | 实际 1024×512；可用于全景背景；3D 天空材质另行设置 | 确认接缝、方向、色彩，不把它当 HDR 光照数据 |
| Cute Cloud / Weather GUI 的 7z | 先解压，再验证 SVG/PNG 及数量 | 这两包目前只验证了归档签名、文件大小与哈希 |

UGUI 卡牌上的费用、标题、描述用文本组件覆盖，不直接沿用源卡面的英文样例字。九宫格拉伸只适合边缘结构允许拉伸的 UI 元件；先设置 Sprite Border 并实际检查结果。

建议测试顺序：显示一张卡→加一个天气状态→显示云敌人→点击牌播放雷击→显示两条地图分支→切换雾天背景。全部通过再扩展素材范围。

## Game Development Studio 交接

当前环境没有 `game-dev` 命令，本仓库不是该工具生成的 canonical package，没有伪造 receipt 或 vendor lock。`manifest.json` 只是本次下载文件校验清单。

以后将这里的素材接入正式游戏项目时，应按 Game Development Studio 的 package 验证与 admission 流程另行处理；不要对本目录直接声称通过 `game-dev package verify`。这次没有修改任何 Unity Assets、Packages 或 ProjectSettings。

Unity 官方设置参考：
- https://docs.unity3d.com/6000.0/Documentation/Manual/texture-type-sprite.html
- https://docs.unity3d.com/6000.0/Documentation/Manual/9SliceSprites.html

## 新增原版资源

[原版素材接入说明](Collections/sts-original/IntegrationNotes.md)：Spine3.4骨骼、图集依赖、原特效图表与音频检查。不要把本批原角色图集当单张人物Sprite，也不要把文件完整性当作Unity兼容性通过。
