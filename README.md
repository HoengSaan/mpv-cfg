# mpv-cfg
My MPV configuration based on [MPV-Lazy](https://github.com/hooke007/MPV_lazy).

IPTV from [IPTV-JP](https://github.com/luongz/iptv-jp/blob/main/jp.m3u), adjusted for personal use.
New shortcut for watching IPTV.

## Localization
Default Language: Traditional Chinese

### English Menu
Rename/Replace input_en.conf to input_uosc.conf in portable_config
Rename/Replace lang_en.lua to lang.lua in portable_config/scripts/uosc/lib

## Basic Key Map
For detail keybind read input_uosc.conf or press Ctrl+i in MPV.
- **F1 ~ F4:** VS Filter
- **F5:** Quick Shortcut for YouTube Clips. (Step: Copy --> F5 --> Paste --> Enter)
- **F6:** Quick Shortcut for Playlist. (Step: F6 --> Playlist Index --> Enter)
- **F7:** Show Current Playlist
- **F8:** Show Current Media Trucks (Audio, Video, Subtitle)
- **F9:** Show Current VS Filter and Equalizer.
- **Ctrl + [1 ~ 6]:** GLSL Filter

## VS Filter
https://github.com/hooke007/MPV_lazy/wiki/3_K7sfunc
VS濾鏡本人使用RIFE補幀，再以ESRGAN超分。
不推薦使用MVTools，有畫面撕裂問題。

Ctrl+0 to Remove All VS Filter
Preset tuned for NVIDIA RTX 4070 Super
Only for Anime.
### Standard Preset
- F1 LD(360p)→QHD(1440p) 4×RES 2×FPS
- Ctrl+F1 SD(480p)→QHD(1440p) 3×RES 2×FPS
- F2 TV(540p)→FHD(1080p) 2×RES 2×FPS
- F3 HD(720p)→QHD(1440p) 2×RES 2×FPS
- F4 FHD(1080p)→UHD(2160p) 2×RES 2×FPS

## GLSL Filter
https://hooke007.github.io/unofficial/mpv_shaders.html
配置允許下建議使用VS濾鏡預設。
Use VS Filter Preset if your spec allow.
Default Anime 4K (High) Preset
https://github.com/bloc97/Anime4K/blob/master/md/GLSL_Instructions_Advanced.md
