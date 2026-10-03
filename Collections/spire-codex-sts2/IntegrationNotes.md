# PNG与预渲染动作接入Unity

## 单张图片

复制需要的PNG到Unity项目的目标素材目录，Texture Type设为Sprite (2D and UI)、Sprite Mode设为Single；按显示用途设置Pixels Per Unit和Filter Mode。UI的按钮、费用、生命、说明文字由项目组件实现。九宫格候选需目视确定Border，不能仅由nine_patch文件名推断像素边界。

卡框、插画、能量图与文字为独立层，原尺寸各异；先用实际文件校对中心、比例与边缘再做UI布局。预渲染角色图的原画布尺寸各异，保持中心/脚底对齐后再调整显示比例。

## 已完整转换的动作

每个动作文件夹有sheet_000.png等页和frames.json。图表最长边不超过2048像素，没有缩放或删帧。设Sprite Mode为Multiple，按原帧宽高切图；JSON逐帧提供page、x、y_top、y_unity、width、height、duration_ms。y_top从左上起算，y_unity从左下起算。末页空格不计入帧。

保持frame_data的index顺序，以duration_ms累加设置关键帧时间；不要假定所有帧时长一致。动作如attack/cast应由战斗状态决定是否重播，原WebP的loop字段只是源文件播放元数据。frames.json为交接数据，Unity不会自动读取它生成AnimationClip。

静态人物PNG和这些预渲染动作图表可采用普通Sprite工作流，不依赖Spine运行时；没有包含可编辑骨骼、皮肤更换、IK或角色逻辑。

## 原VFX图表与遮罩

文件名含flipbook但source_frames为1的素材，是原图内排列的图表，未核实格数、顺序与帧率；本轮保持整图，不能套用上述自动转换动作的frames.json规则。遮罩/噪声/粒子形状需要对应的透明或加法材质，再设置粒子/平面行为。

## 验收步骤

1. 先导入一个完整角色PNG、结束回合按钮与雷电部件，检查透明度、尺寸和边缘。
2. 再导入defect/attack动作页，按frames.json检查第一帧、最后一帧、页切换与总时长。
3. 将费用/生命等文字放在独立文本层，按钮连接项目行为。
4. 最后逐项检查VFX遮罩、混合方式和小图可读性。上述Unity步骤未在本环境执行。

参考：Unity图片导入文档 https://docs.unity.com/en-us/engine/6000.5/manual/materials-and-shaders/textures/importing-textures
