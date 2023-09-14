# GhostCut_Remove_Video_Text
Remove any video text by auto OCR and inpainting. Auto erase video watermarks、texts 、subtitles、logos、emojis...

## [English Version](https://github.com/JollyToday/GhostCut_Remove_Video_Text/blob/main/README.md "GhostCut Video text removal info") --- [中文介绍](https://github.com/JollyToday/GhostCut_Remove_Video_Text/blob/main/README_cn.md "鬼手剪辑去字幕中文介绍")

## Introduction to GhostCut
GhostCut is an intelligent video editing tool. The core purpose is to help users improve the processing speed of materials and the quality of video creative production. It uses a lot of AI capabilities in the processing details of various audio & video, improving the processing efficiency for many video.

Experience address:[Free Try GhostCut Video Text Removal](https://jollytoday.com/Smart_Text_Removal?redirect=%2Fhome&code=th741 "Free Try GhostCut Video Text Removal")

There are Chinese and English versions. Mainland users can access product in  WeChat mini program, search GhostCut.

### Smart Text Removal- video demos
<img src="https://github.com/JollyToday/GhostCut-auto_video_translation/blob/main/4AF80FA6-B2CE-44A0-9123-CEE40423CC60.GIF" width="720"> 

This is Smart Text Removal and Video Inpainting demo video. If you need to learn about video inpainting, please to visit the video inpainting introduction. Compared to other text removal software, such as Runway's Inpainting feature, GhostCut's text removal（Inpainting） is simpler, smarter, and more affordable. You can check the specific differences between GhostCut and Runway in Video Inpainting here: [Difference between GhostCut and Runway in Video Inpainting](https://ghostcut.notion.site/Difference-between-GhostCut-and-Runway-in-Video-Inpainting-f5764304757f4bb995aff2c48fb148a7 "Difference between GhostCut and Runway in Video Inpainting")。

### 1.What kind of video texts can GhostCut automatically remove?

Specifically as follows 

<img src="https://gc100.cdn.izhaoli.cn/ve_material_image/a0b03034fcbd457c/1680243681313.png" width="720">

### 2.Related Video text removal scenarios:

All text in the video is detected by intelligent OCR , and inpainting is applied to restore the video again.

* Any English or Chinese、Japanese、Korean、Arabian subtitle、caption、text、word、copywriting and hardcode subtitles
* Video up and down area with black filling and covered text
* Floating/moving watermark (text)
* Chinese and English watermarking (in the middle of the video, achieved by erasing the video)
* Logo and sticker removal

### 3.Supported Languages for Video OCR and Text Removal
Remove both Chinese and English at the same time, or remove Chinese, English, Japanese, Korean, and Arabic separately; 


### 4.Text Removal and Video Inpainting Details

* Support automatic text removal, first mark the area and only automatically remove the text in marked area, remove all after marking the area, adjust the protection or erasure area and re-synthesize
* Support automatic detection of video subject and upper and lower edges, and refill the background outside the video main subject

### 5.Difference between Smart text removal and Video remover
GhostCut offers two types of video remover products. Smart text removal can automatically remove Chinese and English text from videos, and video remover can remove any objects by manually marking the removal positions through the web version or APIs.

The [Smart Text Removal] of GhostCut also use AI Remover tech but first detects the text in the video and then erases it automatically. If you want to remove some specific logos, stickers or watermarks from the video, you need to use the manual marking method to remove them.

At present, the [Video Remover] function has been released on both the Mini Program side and the PC section of GhostCut. You can directly select any element you want to remove, and the following elements can be removed.[Text] [Icon] [logo] [ watermark ] [logo] [sticker] [animation] and so on…

Compared to other Remover software, such as Runway's Inpainting feature, GhostCut's Inpainting is simpler, smarter, and more affordable. You can check the specific differences between GhostCut and Runway in Video Inpainting here: Difference between GhostCut and Runway in Video Inpainting

## Video Text Removal API interface support
GhostCut provides the output of all API functions, including video deduplicate editing, automatic text removal, video erasure, video subtitle translation, video voice translation (including dubbing) and other interfaces. Multiple capabilities can be superimposed and selected together. (AppKey required)

It can be integrated into third-party products (of course, it is not necessary to develop or have other alternatives, after all, this is a fee).

Such as: Smart Text Removal: https://api.zhaoli.com/v-w-c/gateway/ve/work/fast

**Video Text Removal API Request example**

```json
{"callback":"https://xxx.com/tool/api/ghost-cut/call-back","music":2,"musicRegion":"","needChineseOcclude":1,"needCrop":0,"needMask":0,"needMirror":0,"needRescale":0,"needShift":0,"needTransition":0,"needTrim":0,"outUserId":"624585","randomBorder":0,"resolution":"720p","uid":"xxx","urls":["https://v.douyin.com/Sqv7vgw/"]}
```

**Video Text Removal API Response Example**
```json
{"msg":"success","trace":"c178bdf50dd7454e8db672f0e44593c4","code":1000,"body":{"idProject":220925302,"dataList":[{"url":"https://v.douyin.com/Sqv7vgw/","id":476993630}]}}
```
[API documents](https://jollytoday.feishu.cn/docx/LSNzdoGtOoTSqsxM4K8cooc7nAc "GhostCut API documents")


## Text removal supports the following four modes, and you can customize the protection area or specify the deletion area:

> a. Automatic text removal

> b. First mark the specified area, and then automatically remove the text in the specified area

> c. First mark the area, and then remove all the contents of the marked area

> d. After removing the text, adjust the specified area later

![image](https://github.com/JollyToday/GhostCut_Remove_Video_Text/assets/128401459/383e1eb1-eaf4-458e-94f5-8eb0ed44c190)

![image](https://github.com/JollyToday/GhostCut_Remove_Video_Text/assets/128401459/09bc48c1-412c-4561-9cdb-dd500c7d7983)

* [GhostCut User Guides](https://ghostcut.notion.site/5df83fa6726747b39bd4272a052c1bc1?v=7afb54a3dc70455a949d3945bb0c4221 "GhostCut User Guides")


## Contact GhostCut
* WeChat: 360254, please indicate GitHub in the remark.
* Email：niumoz#izhaoli.com（#-->@）

