# Unity取用与卡牌拖尾参考

此处是接入建议，尚未在Unity项目中执行。没有3D模型或引擎预制体。

| 文件类型 | 建议取用方式 | 当前限制 |
|---|---|---|
| HD敌人/教程PNG | Texture Type=Sprite (2D and UI)，单张Sprite，保留透明度；按站位统一显示高度而非强行等比例外框 | 静态立绘，无骨骼/帧动画 |
| Game-icons透明PNG | 使用白色透明PNG，通过Image.color改成金色/冷色；先在32、64、128px检查可读性 | 最细纹理在小尺寸可能消失 |
| 原SVG | 保存编辑源；已有配套PNG可直接作为普通Sprite导入 | 未安装或验证Vector Graphics包 |
| Nue粒子PNG | 单帧粒子形状或提示Sprite，用发射、缩放和透明度表现效果 | 不按多帧动画切分，无预制体/材质 |
| Buttons-Sheet | 原图256×512，按图形实际区域手工切分，不假定均匀网格 | 未生成SpriteRect/9-slice数据 |
| EnemyStatusIcons | 原图384×64，横向6格64×64可作为切分候选，先检查每格内容 | 未做Unity切片/语义绑定 |
| PSD模板 | 在支持PSD图层的绘图软件中编辑，导出8位RGBA PNG，再按需导入Unity | 空卡面模板不是完整卡框；绿虱PSD为16位通道 |
| 420×2048长图与官方截图 | 用于UI稿、配色和布局参考 | 文字和背景已经合成，不直接当UI控件 |

## 拖尾代码中的实际参数

| 来源位置 | 参数 | 迁移意义 |
|---|---|---|
| procedural_card_trail.gd | point_duration=0.72s；min_spawn_dist=10；max_spawn_dist=42 | 拖尾点存活时间和采样距离；Godot像素单位需按Unity画布尺度换算 |
| procedural_card_trail_vfx.tscn | 三层线宽92/68/32；独立渐变与宽度曲线 | 分层暗影、外发光和亮芯；可用多条TrailRenderer或自定义网格带 |
| 同一场景 BigSparks | amount=52，lifetime=1.2，速度18–42，gravity=0 | 低速长寿命大火花；不能将amount直接当Unity每秒发射率 |
| 同一场景 SmallSparks | amount=72，lifetime=0.34，初速上限420，gravity.y=1640 | 短促小火花；需对应Unity速度、重力和寿命语义重新调参 |
| procedural_card_trail_vfx.gd | 显现0.2s；淡出0.45s | 入场、停止跟随和残留消散的生命周期 |
| procedural_card_fly_vfx.gd | 时长随机0.95–1.45；前视偏移0.05；旋转平滑12 | 二次贝塞尔飞行轨迹和朝向；飞行速度还参与进度变化，不能把随机时长直接当实际总播放时间 |

场景的两张贴图依赖未收录，可以自行制作基础光点或在本库选择合适粒子形状。移植时先统一Canvas坐标、曲线采样和停止时机，再接颜色与粒子；以上只提供原参数，没有写Unity C#实现，也没有在Godot或Unity执行示例。

导入参考：[Unity官方纹理导入文档](https://docs.unity.com/en-us/engine/6000.5/manual/materials-and-shaders/textures/importing-textures)。需要在实际项目检查透明边缘、层级、缩放、发光材质、粒子停止和取消拖拽行为。
