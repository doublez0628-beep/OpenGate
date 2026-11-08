# Open Gate 0.9.20

Open Gate 是视频相机应用，目前为小米 17 Pro 实机内测版，支持 4:3 Open Gate 拍摄、手动曝光与对焦、SDR 和设备支持时的杜比视界；其他设备尚未全面验证。

## 下载

前往 [0.9.20 发布页](https://github.com/doublez0628-beep/OpenGate/releases/tag/v0.9.20)，下载 `OpenGate-0.9.20.apk` 安装包和 `OpenGate-0.9.20-source.zip` 源码包。需要 Android 14 或更高版本。GitHub 自动生成的 Source code 压缩包仅包含仓库文件，请使用发布附件中的源码包。

0.9.20 调整背屏取景与录像控件位置、镜头标记和提示动画，并调整背屏对焦与 ISO 刻度。小米 17 Pro 已进行有限实机交互和短录验证；其他设备、全部方向及模式和长时间录像尚未全面验证。短录不作为性能或稳定帧率基准，无法证明掉帧或发热问题已解决。此前杜比视界文件的动态元数据在 FFmpeg 检查中出现解析错误，跨播放器兼容性仍待验证。

## 源码和构建

源码包包含应用代码、构建脚本、实验材料、第三方依赖及许可说明；版本为 0.9.20 / versionCode 49。项目源码许可条款尚未指定；第三方许可见源码包内 licenses 和 dependencies.json。

构建需要 JDK 17、Android API 35 和 build-tools 35，通过 OG_JAVA、OG_BUILD_TOOLS、OG_ANDROID_JAR 配置工具路径后运行 python3 build.py。原开发签名密钥不包含在源码包内；不同签名无法直接覆盖已有安装，卸载可能导致配置丢失。
