# mpv-cfg
MPV configuration based on [MPV-Lazy](https://github.com/hooke007/MPV_lazy). Fully controllable by Keyborad.

IPTV from [IPTV-JP](https://github.com/luongz/iptv-jp/blob/main/jp.m3u), adjusted for personal use.

## Installation 
1. Download newest archive from release and unarchive to destinated path. (Do not need if downloaded already)
2. Download newest portable config directly and replace existing config.
3. For other language, see **"Localization."** For customization, please search the internet.

### Localization
Default Language: Traditional Chinese
To use English UI:
1. Rename/Replace input_en.conf to input_uosc.conf in portable_config
2. Rename/Replace lang_en.lua to lang.lua in portable_config/scripts/uosc/lib

To use Japanese UI:
1. Rename/Replace input_jp.conf to input_uosc.conf in portable_config
2. Rename/Replace lang_en.lua to lang.lua in portable_config/scripts/uosc/lib (In Progress)

## Basic Key Map
For detailed key map:
1. read [input_uosc.conf](https://github.com/HoengSaan/mpv-cfg/blob/main/portable_config/input_uosc.conf) / [input_en.conf](https://github.com/HoengSaan/mpv-cfg/blob/main/portable_config/input_en.conf).
2. press **Ctrl + i** in MPV.
3. press **Tab** and press **4** in MPV.

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

## Subtitle
External subtitle must containing the media filename or else will not be recognize.
Recommend putting subtitles in subfolder. Folder name should be "sub" or "subtitles", if you perfer other naming, you need to edit it in mpv.conf.

### Traditionalization (繁化)
自動繁化是基於OpenType特性，繁化結果不一定正確。
1. [ayaka14732/FanWunMing](https://github.com/ayaka14732/FanWunMing)
2. [GuiWonder/HuayingMincho](https://github.com/GuiWonder/HuayingMincho)
3. [GuiWonder/Shanggu](https://github.com/GuiWonder/Shanggu) （正在使用）
須在電腦安裝自動繁化字體否則無法啓用繁化。如果使用ASS字幕則需按「h」或「Shift + h」鍵強制取代字幕樣式。

## Audio
External audio must containing the media filename or else will not be recognize.

## Preset
https://github.com/hooke007/MPV_lazy/wiki/3_K7sfunc

https://hooke007.github.io/unofficial/mpv_shaders.html

https://github.com/bloc97/Anime4K/blob/master/md/GLSL_Instructions_Advanced.md

Use VS Filter Preset if your spec allow.
This preset is tuned for NVIDIA RTX 4070 Super and only work for anime, and better without hard subtitle (subtitle that are burnt in the video track), always use soft subtitle, either external (inn the folder) or internal (in the container).
This preset use RIFE for frame interpolation and ESRGAN for super resoulution to achieve the best effect.
You can change RIFE to MVTools for lower spec PC. However, MVTools's effect is not as good as RIFE.
If your spec is even lower, use Anime4K instead of ESRGAN.

Use **Ctrl + 0** to remove all alteration.
Use **F9** to check.

### Standard VS Preset
- F1 LD(360p)→QHD(1440p) 4×RES 2×FPS
- Ctrl+F1 SD(480p)→QHD(1440p) 3×RES 2×FPS
- F2 TV(540p)→FHD(1080p) 2×RES 2×FPS
- F3 HD(720p)→QHD(1440p) 2×RES 2×FPS
- F4 FHD(1080p)→UHD(2160p) 2×RES 2×FPS

### Standard Anime4K Preset
- **Ctrl + [1 ~ 6]:** Anime4K High Quality Preset
- **Ctrl + (Shift) + [1 ~ 6]:** Anime4K Low Quality Preset
