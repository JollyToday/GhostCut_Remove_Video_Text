# 鬼手剪辑_智能去字幕和视频擦除
通过自动视频OCR和视频修复，擦除任何视频内的文本。可擦除视频水印、文本、字幕、徽标、表情符号、人物、物体等…

[English Version]（https://github.com/JollyToday/GhostCut_Remove_Video_Text/main/README.md"GhostCut English info") ---- [中文介绍]（https://github.com/JollyToday/GhostCut/blob/main/README_cn.md"鬼手剪辑中文介绍"）

## 鬼手剪辑简介
鬼手剪辑又称为GhostCut，他是一款智能视频编辑工具，核心目的是帮助用户提升素材的处理速度和视频创意制作的质量，在各种音视频的处理细节中使用了大量的AI能力，为很多视频提升了处理效率。

体验地址：【免费体验鬼手剪辑视频去文字】（https://jollytoday.com/Smart_Text_Removal?redirect=%2Fhome&code=th741“免费试用GhostCut视频文字移除”）

软件有中英文版本，提供API支持和私有化部署服务。大陆用户可以在微信小程序中访问产品，搜索GhostCut或鬼手剪辑。

## 智能去字幕-视频演示
<imgsrc="https://github.com/JollyToday/GhostCut-auto_video_translation/blob/main/4AF80FA6-B2CE-44A0-9123-CEE40423CC60.GIF"width="720">

这是智能文本移除和视频修复演示视频。如果您需要了解视频擦除，请访问视频擦除介绍。与其他的擦除和修复软件相比，例如Runway的修复功能，GhostCut的文本移除（修复）更简单、更智能、更实惠。您可以在此处查看GhostCut和Runway在视频修复中的具体区别：【GhostCut和Runway在视频修复中的区别】（https://ghostcut.notion.site/Difference-between-GhostCut-and-Runway-in-Video-Inpainting-f5764304757f4bb995aff2c48fb148a7“GhostCut和Runway在视频修复中的区别”）。

### 1. 鬼手剪辑可以擦除什么样的视频元素？

具体如下

<imgsrc="https://gc100.cdn.izhaoli.cn/ve_material_image/a0b03034fcbd457c/1680243681313.png"width="720">

### 2.相关视频擦除场景有哪些：

鬼手剪辑通过智能OCR检测视频中的所有文本，并应用修复以再次恢复视频。

- 任何英语或中文文字、日语、韩语、阿拉伯语等视频字幕、标题、文本、单词、文案和硬编码的字幕；
- 去除视频上下区域有黑色填充和覆盖文字
- 去除浮动/移动水印（文字）
- 去除中英文logo水印（在视频中间，通过抹除视频实现）
- 去除徽标和贴纸等

### 3.支持的视频OCR和文本删除语言
同时去掉中文和英文，或者分别去掉中文、英文、日文、韩文、阿拉伯文等；

### 4.文本移除和视频修复细节

- 支持文本自动移除，先标记区域后仅自动移除标记区域内的文本，标记区域后全部移除，调整保护或擦除区域后重新合成
- 支持自动检测视频主体和上下边缘，在视频主主体外重新填充背景
更多用法参考后文的擦除应用案例

### 5.智能去字幕和视频擦除的区别
鬼手剪辑提供两种类型的视频擦除/修复产品。智能去文字可以自动从视频中移除中、英等语言字幕，视频擦除可以通过网页版或API手动标记移除位置来移除任何视频内的对象。

GhostCut的[智能去文字]也使用AI Remover技术，他会首先使用视频OCR检测视频中所有的文本，然后自动擦除，在过程中尽量避免擦除商品本身的文字。如果你想从视频中删除一些特定的标志、贴纸或水印，你需要使用手动标记的方法来删除它们。

目前小程序端和GhostCut的PC板块都已经发布了【视频移除】功能，可以直接选择任意想要移除的元素，下面的元素都可以移除。【文字】【图标】【logo】【水印】【logo】【贴纸】【动画】等等…

与Runway的修复功能等其他Remover软件相比，GhostCut的修复更简单、更智能、更实惠。您可以在此处查看GhostCut和Runway在视频修复中的具体区别：GhostCut和Runway在视频修复中的区别

## 视频去字幕和视频擦除的API接口支持
鬼手剪辑提供了所有API功能的输出，包括视频去重编辑、文本自动去除、视频擦除、视频字幕翻译、视频语音翻译（含配音）等界面。多种能力可以叠加在一起选择。（需要AppKey）
可以集成到第三方产品中。

如：智能去文字：https://api.zhaoli.com/v-w-c/gateway/ve/work/fast

智能去除视频字幕API请求示例
```json
{"callback":"https://xxx.com/tool/api/ghost-cut/call-back","music":2,"musicRegion":"","needChineseOcclude":1,"needCrop":0,"needMask":0,"needMirror":0,"needRescale":0,"needShift":0,"needTransition":0,"needTrim":0,"outUserId":"624585","randomBorder":0,"resolution":"720p","uid":"xxx","urls":["https://v.douyin.com/Sqv7vgw/"]}
```

智能去字幕API响应示例
```json
{"msg":"success","trace":"c178bdf50dd7454e8db672f0e44593c4","code":1000,"body":{"idProject":220925302,"dataList":[{"url":"https://v.douyin.com/Sqv7vgw/","id":476993630}]}}
[API文档]（https://jollytoday.feishu.cn/docx/LSNzdoGtOoTSqsxM4K8cooc7nAcGhostCutAPI文档）
```

## 视频擦除类产品支持以下四种模式，你可以自定义保护区域或指定删除区域：

a.自动删除视频内所有检测到的文本

b.先标记指定区域，然后自动擦除指定区域的文字

c.先标记区域，然后移除标记区域的所有内容

d.移除文字后，对指定区域的处理结果进行二次调整，设置保护区域放置误擦除或指定再次擦除。

！[图片]（https://github.com/JollyToday/GhostCut_Remove_Video_Text/assets/128401459/383e1eb1-eaf4-458e-94f5-8eb0ed44c190）

！[图片]（https://github.com/JollyToday/GhostCut_Remove_Video_Text/assets/128401459/09bc48c1-412c-4561-9cdb-dd500c7d7983）

- [GhostCut用户指南]（https://ghostcut.notion.site/5df83fa6726747b39bd4272a052c1bc1?v=7afb54a3dc70455a949d3945bb0c4221GhostCut用户指南）


## 联系GhostCut
- 微信：360254，备注请注明GitHub。
- 邮箱： niumoz#izhaoli.com (#-->@)

