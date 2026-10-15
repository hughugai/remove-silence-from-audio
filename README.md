---
title: Remove Silence From Audio
emoji: 📉
colorFrom: indigo
colorTo: gray
sdk: gradio
sdk_version: 6.30.0
python_version: '3.12'
app_file: app.py
pinned: false
license: apache-2.0
short_description: '[silenceremove.com](https://silenceremove.com)'
---

# 😻 Remove Silence From Audio

Upload an Audio file, and it will remove silent parts from it.

**🌐 免费在线音频工具（无需安装）：[silenceremove.com](https://silenceremove.com/)**

## 本地运行

```bash
pip install -r requirements.txt
python app.py
```

依赖系统安装 [ffmpeg](https://ffmpeg.org/)。启动后访问 http://localhost:7860

## 功能

- 上传或麦克风录音，自动检测并移除静音片段
- 支持 mp3 / wav / ogg / flac / m4a 等格式（ffmpeg 自动转 wav）
- 可设置每段保留的静音时长（秒），避免语速过于急促
- 静音过响时自动改用动态阈值（相对整体响度 -16dB）
- 显示处理前后时长对比，临时文件每小时自动清理

Check out the configuration reference at https://huggingface.co/docs/hub/spaces-config-reference
