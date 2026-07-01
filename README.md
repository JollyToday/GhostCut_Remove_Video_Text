# GhostCut_Remove_Video_Text
Remove any video text by auto OCR and inpainting. Auto erase video watermarks、texts 、subtitles、logos、emojis...

## [English Version](https://github.com/JollyToday/GhostCut_Remove_Video_Text/blob/main/README.md "GhostCut Video text removal info") --- [中文介绍](https://github.com/JollyToday/GhostCut_Remove_Video_Text/blob/main/README_cn.md "鬼手剪辑去字幕中文介绍")

> **International users:** Use [Weydub Subtitle Removal](https://weydub.com/subtitle-removal/) and the [Video Subtitle Removal API guide](https://weydub.com/docs/api/video-subtitle-removal.html). Weydub is the international version of GhostCut; this repository keeps the historical GhostCut project name for compatibility, and older screenshots/GIFs may still show the original domestic brand.

## Introduction to Weydub
Weydub, the international version of GhostCut, is an intelligent video editing and localization tool. The core purpose is to help users improve material processing speed and video creative production quality. It uses AI capabilities across audio and video processing details, improving efficiency for many video workflows.

Experience address:[Try Weydub Subtitle Removal](https://weydub.com/subtitle-removal/ "Try Weydub Subtitle Removal")

For international users, use Weydub on the web. Mainland China users can still access the domestic GhostCut product in the WeChat mini program.

### Smart Text Removal- video demos
<img src="https://github.com/JollyToday/GhostCut-auto_video_translation/blob/main/4AF80FA6-B2CE-44A0-9123-CEE40423CC60.GIF" width="720"> 

This is a smart text removal and video inpainting demo. Compared to other text removal software, such as Runway's inpainting feature, Weydub/GhostCut text removal is designed to be simple, smart, and cost effective. You can start from [Weydub Subtitle Removal](https://weydub.com/subtitle-removal/ "Weydub Subtitle Removal").

### 1.What kind of video text can Weydub automatically remove?

Specifically as follows 

<img src="https://gc100.cdn.izhaoli.cn/ve_material_image/A-a0b03034fcbd457c/c2fef7a4532d4effb7ce2b0214d0ad66/1711978895360.png" width="720">

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
Weydub/GhostCut offers two types of video remover products. Smart text removal can automatically remove Chinese and English text from videos, and video remover can remove any objects by manually marking the removal positions through the web version or APIs.

The [Smart Text Removal] workflow uses AI remover technology, but first detects the text in the video and then erases it automatically. If you want to remove some specific logos, stickers or watermarks from the video, you need to use the manual marking method to remove them.

At present, the [Video Remover] function is available in the domestic GhostCut product and related web/API flows. You can directly select any element you want to remove, and the following elements can be removed.[Text] [Icon] [logo] [ watermark ] [logo] [sticker] [animation] and so on…

Compared to other remover software, such as Runway's inpainting feature, Weydub/GhostCut inpainting is designed to be simpler, smarter, and more affordable. Start from [Weydub Subtitle Removal](https://weydub.com/subtitle-removal/).

## Video Text Removal API interface support
Weydub provides API access for video localization workflows, including automatic text removal, video erasure, video subtitle translation, video voice translation (including dubbing), and related interfaces. Multiple capabilities can be superimposed and selected together. (AppKey required)

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
[Video Text Removal API documents](https://weydub.com/docs/api/video-subtitle-removal.html "Weydub Video Text Removal API documents")


## Text removal supports the following four modes, and you can customize the protection area or specify the deletion area:

> a. Automatic text removal

> b. First mark the specified area, and then automatically remove the text in the specified area

> c. First mark the area, and then remove all the contents of the marked area

> d. After removing the text, adjust the specified area later

![image](https://github.com/JollyToday/GhostCut_Remove_Video_Text/assets/128401459/383e1eb1-eaf4-458e-94f5-8eb0ed44c190)

![image](https://github.com/JollyToday/GhostCut_Remove_Video_Text/assets/128401459/09bc48c1-412c-4561-9cdb-dd500c7d7983)

[Weydub API and automation guides](https://weydub.com/docs/api/ "Weydub API and automation guides")

## More about Weydub and GhostCut APIs
- Weydub is the international version of GhostCut for web product access, API docs, and automation guides.
- Weydub/GhostCut API advantages: Focus on AI video, has served many users, and is trusted by API customers at home and abroad. Good product experience, strong results, cost effective, support private deployment and partial customization, support secondary editing, and provide dedicated integration support.
- Weydub/GhostCut API provides capabilities including video inpainting (de-text), video deduplication, video eraser, video translation (by ASR), video translation (by OCR), AI dubbing, template editing, video segmentation, video OCR and other interfaces. Multiple capabilities can be combined in one interface. If you need more, please contact us.

## Contact
* For international product access, start from [Weydub](https://weydub.com/).
* WeChat: 360254, please indicate GitHub in the remark.
* Email：niumoz#izhaoli.com（#-->@）
