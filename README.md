# mpv-cfg
My MPV configuration based on [MPV-Lazy](https://github.com/hooke007/MPV_lazy).

IPTV from [IPTV-JP](https://github.com/luongz/iptv-jp/blob/main/jp.m3u), adjusted for personal use.
New shortcut for watching IPTV.

## VS濾鏡
https://github.com/hooke007/MPV_lazy/wiki/3_K7sfunc
VS濾鏡本人使用RIFE補幀，再以ESRGAN超分。
不推薦使用MVTools，有畫面撕裂問題。

F1清空。以下預設皆需NVIDIA顯卡。
### 預設（雙倍幀數超分）
- SD480P超分至QHD1440P **F1**
- HD720P超分至QHD1440P **F2** 標準
- HD720P超分至UHD2160P **F3**
  - 經本人測試4070Super並不能流暢播放，效果和標準差異並不大。
- FHD1080P超分至UHD2160P **F4**
  - 使用4070Super可流暢播放。

## 着色器
https://hooke007.github.io/unofficial/mpv_shaders.html
配置允許下建議使用VS濾鏡預設。
預設與Anime4K無異。
https://github.com/bloc97/Anime4K/blob/master/md/GLSL_Instructions_Advanced.md
