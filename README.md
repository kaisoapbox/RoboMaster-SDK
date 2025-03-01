# RoboMaster-SDK

OK SO to build this from source what you gotta do is:

1. You probably need FFMpeg and Opus installed. You also need CMake. I used homebrew for both.
2. Update `lib/libmedia_codec/CMakeLists.txt` with the paths to your libraries, because I hardcoded everything lmao.

```bash
cd lib/libmedia_codec
pip install .
cd ../..
pip install .
```

This should build both the `robomaster` library and the `libmedia_codec` library (which `robomaster` depends on, and I couldn't figure out how to build and bundle properly). If you encounter errors, god help you.

This worked for me on MacOS arm64, python 3.13, with ffmpeg and opus installed and versions _mumble mumble mumble_.

## their old random stuff

[![Gitter](https://badges.gitter.im/RoboMaster-SDK/community.svg)](https://gitter.im/RoboMaster-SDK/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

<img src="docs/source/images/robomaster.jpg" width="600">

Learn more about the RoboMaster Education Robot: https://www.dji.com/robomaster-ep

RoboMaster Developer Guide: https://robomaster-dev.rtfd.io/

Gitee link for RoboMaster SDK download: https://gitee.com/xitinglin/RoboMaster-SDK
