
# Open Gate 0.9.6

Open Gate 是视频相机应用，目前为小米 17 Pro 实机内测版。支持 4:3 Open Gate 拍摄、手动曝光与对焦、SDR 和设备支持时的杜比视界；其他设备的支持情况尚未验证。

## 下载

请前往 [0.9.6 发布页](https://github.com/doublez0628-beep/OpenGate/releases/tag/v0.9.6) 下载 APK 安装包和对应源码包 `OpenGate-0.9.6-source.zip`。需要 Android 14 或更高版本。GitHub 自动生成的 Source code 压缩包仅包含仓库文件，请使用附带的源码包。

0.9.6 统一了分辨率菜单图标，并保留 0.9.5 的重复尺寸去除。三摄色彩匹配尚未完成，与系统相机的画质差距尚未解决。

## 源码和构建

源码包包含应用代码、构建脚本、第三方依赖及许可说明。源码包内 README 标题仍写 0.9.4，实际版本以 AndroidManifest.xml 中的 0.9.6 / versionCode 35 为准。项目源码许可条款尚未指定；第三方许可见源码包内 licenses 和 dependencies.json。

构建需要 JDK 17、Android API 35 和 build-tools 35，通过 OG_JAVA、OG_BUILD_TOOLS、OG_ANDROID_JAR 配置工具路径后运行 python3 build.py。原开发签名密钥不包含在源码包内；不同签名无法直接覆盖已有安装，卸载可能导致配置丢失。
