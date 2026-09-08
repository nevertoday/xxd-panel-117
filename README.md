<div align="center">

# XXD Panel 117｜细线淡彩留白志

以一个视觉锚点，重新安排照片里的主题与留白

<strong>简体中文</strong> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

## 样张展示

以下样张均来自不同的原始参考图，由 Panel 117 独立单轮生成，并已清理 AI 元数据。横版严格为左侧原图、右侧设计，各占 50%；竖版严格为上方原图、下方设计，各占 50%。

样张从不同素材目录选择原图，分别生成与内容相关的英文智能文案。

**16:9 横版 · 左右 50:50**

| sample-05 | sample-06 |
|---|---|
| ![sample-05](assets/examples/sample-05.png) | ![sample-06](assets/examples/sample-06.png) |
| ![sample-07](assets/examples/sample-07.png) | ![sample-08](assets/examples/sample-08.png) |

**3:4 竖版 · 上下 50:50**

| sample-09 | sample-10 |
|---|---|
| ![sample-09](assets/examples/sample-09.png) | ![sample-10](assets/examples/sample-10.png) |
| ![sample-11](assets/examples/sample-11.png) | ![sample-12](assets/examples/sample-12.png) |

## 适用场景与解决的问题

当照片杂乱、构图平常，但仍有一个值得留下的主题时，**Panel 117** 会先找出一个核心主题、一个视觉锚点和一种情绪关系，再把它们重新导演成细线、淡彩、纸张肌理与轻拼贴组成的小尺度画面。真实照片仍可保留在对照区，设计区通过大面积有意识留白获得独立表达。

### 适合这些情况

- 希望保留原物辨识度，同时重新安排主体的位置、尺度、方向和裁切。
- 不想逐物描摹或保留杂乱背景，需要少元素、强主题的艺术海报。
- 喜欢轻薄线条、柔和粉彩与纸面呼吸感，避免写实细节和光滑矢量。
- 需要同一风格输出上下、左右、纯设计、多比例、四端壁纸或目录批处理。

### 它替你解决什么

- 从复杂素材中选出真正重要的视觉锚点，删除次要信息。
- 让留白参与正负形、距离与不对称平衡，而非把画面填满。
- 对照图严格只有两个各占 50% 的区域，不出现第三带或内嵌面板。
- 每个输出从当前原图独立单轮生成，避免中间结果再次转绘。

## 原始提示词 · 五种语言

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

中文文件逐字保存用户原文，是运行时唯一的创作与审美权威；其他四语是完整忠实的阅读译文。明确选择左右等非默认模式时，适配器仅映射交付位置与尺寸，原文审美不变。

**关键词：** 一个核心主题 · 一个视觉锚点 · 一种情绪关系 · 细线手绘 · 淡彩平涂 · 纸张肌理 · 轻拼贴 · 小尺度章印 · 2–4 色 · 大留白 · 纤细手写字

## 快速判断：Panel 117 适合你吗？

| 你关心的问题 | 这套风格给你的回答 |
|---|---|
| 原照片构图普通也能用吗？ | 可重设主体大小、位置、方向与裁切，提炼后重构。 |
| 极简后还能认出原物吗？ | 保留最有代表性的轮廓、走势、姿态和视觉记忆点。 |
| 留白只是没有画满吗？ | 留白明显大于绘制面积，并主动组织距离与正负形。 |
| 需要多种交付尺寸？ | 支持常用比例、准确像素、四种模式和目录批量。 |

## 它如何把照片变成成品

```text
识别一个主题、锚点与情绪关系 → 删除其余信息 → 重设主体尺度、位置和裁切 → 细线与淡彩平涂重构 → 以浅色块、纸纹和轻拼贴组织关系 → 用大留白与少量手写字完成
```

## 成品中最容易识别的特点

- 主体由少量简洁细轮廓识别，内部只有极少必要线条。
- 轻薄平静的色面取代写实细节；可用一块极浅主题色承托，主体允许越过其边缘。
- 小尺度章印式主体可偏心、贴边、悬置或局部裁切；留白面积明显大于绘制面积。
- 从原图提取 2–4 色并调为高明度、清透柔和的粉彩，近白纸底保持清晰对比。
- 极少符号来自主题或情绪，以一两笔表达，不复制真实物件或为填空装饰。
- 少量文字源于主体、动作、情绪、记忆或隐喻，以纤细自然、略带手写感的字体融入余白。

## 四种输出模式

- `top-bottom`：整张画布只有上下两个全宽区域，现实照片在上、设计在下，严格各占 50%。
- `left-right`：整张画布只有左右两个全高区域，现实照片在左、设计在右，严格各占 50%，不会旋转成上下结构。
- `design-only`：整张画布只呈现 Panel 117 的设计转译，照片只作为不可见参考。
- `wallpaper-pack`：按手机、iPad、桌面和手表分别生成完整设计壁纸，可选 `linked` 连贯套装或 `independent` 四张独立。

支持多选模式与比例（`1:1`、`3:4`、`4:3`、`4:5`、`5:4`、`2:3`、`3:2`、`9:16`、`16:9`、`21:9`、`5:7`、`7:5` 或准确像素），以及模型生成文字、准确文字和无文字。传入目录会递归扫描图片，每张源图独立处理，共用一次交付设置；最终 PNG 平铺放入一个新任务目录。

## 开始使用

```bash
git clone https://github.com/nevertoday/xxd-panel-117.git
npx skills add https://github.com/nevertoday/xxd-panel-117 --skill xxd-panel-117
```

安装后重新启动 Agent 会话，然后调用 `$xxd-panel-117`。也可以按需追加 `--global --agent codex --yes` 做用户级安装。

常用调用示例：

```text
/xxd-panel-117 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale zh-CN
/xxd-panel-117 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-117 photo.jpg --mode design-only --size 9:16 --text none
/xxd-panel-117 ./photos --mode design-only --size auto,3:4 --text prompt --locale ja-JP
```

完整运行契约见 [SKILL.md](SKILL.md)；运行适配器见 [英文](references/xxd-panel-117-prompt.en.md) 与 [中文](references/xxd-panel-117-prompt.zh-CN.md)。

<!-- xxd-readme-ads:start -->
## 关于 XXD

XXD 是小小东品牌名的缩写，本项目由小小东创建并维护： [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## 广告信息｜XXD 付费服务与会员

> **广告与商业信息声明：** 以下二维码、会员与付费服务链接属于小小东的广告信息。是否扫码或购买完全自愿，不影响本开源项目的访问与使用。


<!-- xxd-panel-command-system:start -->

将军 Skills 已包含在 699 元/年的统一会员权益中，无需单独购买。

| 层级 | Skill | 负责什么 |
|---|---|---|
| **将军级** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | 识别当前可用的编号 Skills；按图片、主题和用途推荐；按编号点将；组织同图多风格试稿；为图片文件夹批量分配并逐项派发。 |
| **士兵级** | `xxd-panel-NNN` | 每个编号只执行自己独立的原始提示词与审美，把将军派发的单个任务完成为成品。 |

<!-- xxd-panel-command-system:end -->

### 知识星球＋成员提示词库＋Skills 所有将军会员 · 699 元/年

[知识星球](https://wx.zsxq.com/group/15554814142882)、[小小东成员提示词库](https://vip.xiaoxiaodong.ai/)与 Skills 所有将军会员是同一份会员权益：**一次年费同时开通三项权益，无需重复付费。**

[Knowledge Planet](https://wx.zsxq.com/group/15554814142882) · [Member Prompt Library](https://vip.xiaoxiaodong.ai/)

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD WeChat" width="280"></a></p>
<!-- xxd-readme-ads:end -->

## 许可证

本项目（包括 Skill、提示词、脚本、文档及随附样张）采用 **PolyForm Noncommercial License 1.0.0**。完整法律条文请见 [LICENSE](LICENSE)，官方页面见 <https://polyformproject.org/licenses/noncommercial/1.0.0>。

用人话说：

- 个人可以用于学习、研究、实验、测试、兴趣项目和私人娱乐；慈善机构、教育机构、公共研究/安全/卫生机构、环保组织及政府机构也可以使用。
- 在**非商业目的**下，你可以使用、复制、修改、制作衍生作品并分享；分享时必须同时提供本许可证（或上面的链接）以及作者提供的所有 `Required Notice:` 声明。
- 不允许用于商业产品或服务、收费交付、出售访问权或许可，或任何预期会带来商业应用的用途。需要商业使用时，请先向版权方另行取得书面许可。
- 本协议只授予其中明确写出的著作权许可和有限的专利许可，不授予商标、品牌名称或其他未明确授予的权利，也不能把你的许可再转授给他人。
- 如果收到书面违约通知，须在 32 天内纠正并采取实际补救措施，否则许可会立即终止；就专利侵权提出书面主张也会终止专利许可。
- 内容按“现状”提供，在法律允许的范围内不作任何担保，使用风险和可能的损失由使用者自行承担。
