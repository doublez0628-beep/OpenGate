# Open Gate 0.9.11

Open Gate 是视频相机应用，目前为小米 17 Pro 实机内测版，支持 4:3 Open Gate 拍摄、手动曝光与对焦、SDR 和设备支持时的杜比视界；其他设备尚未验证。

## 下载

前往 [0.9.11 发布页](https://github.com/doublez0628-beep/OpenGate/releases/tag/v0.9.11)，下载 APK 安装包和 `OpenGate-0.9.11-source.zip` 源码包。需要 Android 14 或更高版本。GitHub 自动生成的 Source code 压缩包仅包含仓库文件，请使用发布附件中的源码包。

0.9.11 修复四摄连拍音量键短按时倍率显示重复及跳档，短按每次调整 0.1×，长按延时后连续变焦；包含 0.9.10 的背屏点击修复。小米 17 Pro 上通过 USB 模拟按键对指定倍率及录像进行了有限验证，实体按键手感、其他模式及其他设备未在本版复测。镜头切换取决于系统和条件；原有 HDR 录像期间前后摄切换限制仍在。

## 源码和构建

源码包包含应用代码、构建脚本、第三方依赖及许可说明。源码包内 README 标题仍写 0.9.4，实际版本以 AndroidManifest.xml 中的 0.9.11 / versionCode 40 为准。项目源码许可条款尚未指定；第三方许可见源码包内 licenses 和 dependencies.json。

构建需要 JDK 17、Android API 35 和 build-tools 35，通过 OG_JAVA、OG_BUILD_TOOLS、OG_ANDROID_JAR 配置工具路径后运行 python3 build.py。原开发签名密钥不包含在源码包内；不同签名无法直接覆盖已有安装，卸载可能导致配置丢失。
