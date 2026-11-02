# Open Gate 0.9.9

Open Gate 是视频相机应用，目前为小米 17 Pro 实机内测版，支持 4:3 Open Gate 拍摄、手动曝光与对焦、SDR 和设备支持时的杜比视界；其他设备尚未验证。

## 下载

前往 [0.9.9 发布页](https://github.com/doublez0628-beep/OpenGate/releases/tag/v0.9.9)，下载 APK 安装包和 `OpenGate-0.9.9-source.zip` 源码包。需要 Android 14 或更高版本。GitHub 自动生成的 Source code 压缩包仅包含仓库文件，请使用发布附件中的源码包。

0.9.9 将“三摄联动”更名为“四摄连拍”，支持该模式音量键变焦，以及背屏单击开始或停止录像。小米 17 Pro 已进行有限验证，用户已确认实体按键和背屏手指操作及调整后的变焦速度；独立主摄仅验证系统音量调节请求，音量值未核实。其他设备未测试，原有 HDR 录像期间前后摄切换限制仍在。

## 源码和构建

源码包包含应用代码、构建脚本、第三方依赖及许可说明。源码包内 README 标题仍写 0.9.4，实际版本以 AndroidManifest.xml 中的 0.9.9 / versionCode 38 为准。项目源码许可条款尚未指定；第三方许可见源码包内 licenses 和 dependencies.json。

构建需要 JDK 17、Android API 35 和 build-tools 35，通过 OG_JAVA、OG_BUILD_TOOLS、OG_ANDROID_JAR 配置工具路径后运行 python3 build.py。原开发签名密钥不包含在源码包内；不同签名无法直接覆盖已有安装，卸载可能导致配置丢失。
