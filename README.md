# mpv-cfg
MPV configuration based on [MPV-Lazy](https://github.com/hooke007/MPV_lazy). Fully controllable by Keyborad.

IPTV from [IPTV-JP](https://github.com/luongz/iptv-jp/blob/main/jp.m3u), adjusted for personal use.

## Installation 安裝
1. Download newest archive from release and unarchive to destinated path. (Do not need if downloaded already)
2. Download newest portable config directly and replace existing config.

1. 從Release中下載最新版本竝解壓至目標路徑。（如已有狹窄則不需）
2. 下載最新Portable Config竝取代已有Config。

### Localization 本地化
Default Language（默認語言）: English

To change language, open **"portable_config/mpv.conf"** with a text editor such as Notepad++, and change "input-conf" to your intended language.

欲想更改語言，請用諸如Notepad++等文本編輯器開啓「portable_config/mpv.conf」，然後將「input-conf」改成閣下欲用語言。

#### English
```
input-conf = "~~/input_en.conf" #English
```

#### Traditional Chinese
```
input-conf = "~~/input_tc.conf" #Traditional Chinese
```

#### Japanese
```
input-conf = "~~/input_jp.conf" #Japanese
```

## Basic Key Map 基本鍵圖

- **F1 ~ F4:** VS Filter Preset, see **"Preset"** for details
- **F5:** Quick Shortcut for YouTube Clips (Step: Copy --> F5 --> Paste --> Enter)
- **F6:** Quick Shortcut for Playlist (Step: F6 --> Playlist Index --> Enter)
- **F7:** Show Current Playlist
- **F8:** Show Current Media Trucks (Audio, Video, Subtitle)
- **F9:** Show Current VS Filter, Equalizer and other important information
- **Tab:** Toggle Stat Display
- **Ctrl + (Shift) + [1 ~ 6]:** GLSL Shader Preset, see **"Preset"** for details
- **Alt + [1 ~ 7]:** MEMC RIFE NV
- **Shift + [1 ~ 6]:** SR ESRGAN NV
- **[1 ~ 0]:** Window Adjustment
- **[q ~ p]:** Equalizer

For detailed key map 詳細見圖請見:
1. read the config instead.
2. press **Ctrl + i** in MPV.
3. press **Tab** and press **4** in MPV.

## Subtitle 字幕
External subtitle must containing the media filename or else will not be recognize.
Recommend putting subtitles in subfolder. Folder name should be "sub" or "subtitles", if you perfer other naming, you need to edit it in mpv.conf.

外掛字幕必須包含媒體文件名、否則將無法識別。
推薦將字幕放於子文件夾中，竝命名爲「sub」或「subtitles」，若閣下欲用其他命名方式，則須在「mpv.conf」中修改。

### Traditionalization 繁化
自動繁化是基於OpenType特性，繁化結果不一定正確。
1. [ayaka14732/FanWunMing](https://github.com/ayaka14732/FanWunMing)
2. [GuiWonder/HuayingMincho](https://github.com/GuiWonder/HuayingMincho)
3. [GuiWonder/Shanggu](https://github.com/GuiWonder/Shanggu) （正在使用）

須在電腦安裝自動繁化字體並在input.conf設定，否則無法啓用繁化。如果使用ASS字幕則需按「h」或「Shift + h」鍵取代字幕樣式。可使用Nexusfont檢視字體效果。

## Audio 音軌
External audio must containing the media filename or else will not be recognize.

外掛音軌必須包含媒體文件名、否則將無法識別。

## Preset 預設
https://github.com/hooke007/MPV_lazy/wiki/3_K7sfunc

https://hooke007.github.io/unofficial/mpv_shaders.html

https://github.com/bloc97/Anime4K/blob/master/md/GLSL_Instructions_Advanced.md

Use VS Filter Preset if your spec allow.
This preset is tuned for NVIDIA RTX 4070 Super and only work for anime, and better without hard subtitle (subtitle that are burnt in the video track), always use soft subtitle, either external (inn the folder) or internal (in the container).
This preset use **"RIFE"** for frame interpolation and **"ESRGAN"** for super resoulution to achieve the best effect.
You can change **"RIFE"** to **"MVTools"** for lower spec PC. However, **"MVTools"**'s effect is not as good as **"RIFE"**.
If your spec is even lower, use **"Anime4K"** instead of **"ESRGAN"**.

請用VS濾鏡預設若閣下配置允許。
本預設是基於NVIDIA RTX 4070 Super調整，竝祇適用於動畫，且避免使用硬字幕。
本預設使用「RIFE」進行補幀，再以「ESRGAN「進行超分，以達到最佳效果。
若配置較低，可將「RIFE」更改爲「MVTools」，但「MVTools」效果不如「RIFE」。
若配置更差，請使用「Anime4K」取代VS濾鏡。

Use **Ctrl + 0** to remove all alteration.
Use **F9** to check.

### Standard VS Preset 標準VS預設
- **F1** LD(360p)→QHD(1440p) 4×RES 2×FPS
- **Ctrl+F1** SD(480p)→QHD(1440p) 3×RES 2×FPS
- **F2** TV(540p)→FHD(1080p) 2×RES 2×FPS
- **F3** HD(720p)→QHD(1440p) 2×RES 2×FPS
- **F4** FHD(1080p)→UHD(2160p) 2×RES 2×FPS

### Standard Anime4K Preset 標準Anime4K預設
- **Ctrl + [1 ~ 6]:** Anime4K High Quality Preset
- **Ctrl + (Shift) + [1 ~ 6]:** Anime4K Low Quality Preset
