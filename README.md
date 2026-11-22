# FrostShade

FrostShade 是面向 **ColorOS 15** 和 **ColorOS 16** 的 **LSPosed 磨砂液态玻璃模块**。它在通知中心提供可展开的堆叠通知，并为控制中心的原有控件加入磨砂玻璃效果。两项功能可以分别开启。

## 效果演示

![磨砂液态玻璃通知从堆叠到展开，再收起](https://raw.githubusercontent.com/MuYuanXing/FrostShade/main/docs/notification-stack-preview.gif)

## 功能

### 通知中心

- **磨砂堆叠通知**。点开一组通知即可查看组内卡片。支持按同一组、同一应用或全部通知堆叠。
- **布局与排序**。可调整堆叠层数、卡片露出高度和大小，支持按时间、应用名、重要性或卡片高度排序。
- **玻璃与光效**。可调整背景模糊、卡片表面浓度、阴影和亮边，并按需开启按压光效、流光和氛围光。

### 控制中心

- 为快捷开关等原有控件加入磨砂玻璃外观。
- 可开启并调节浅色模式下的额外压暗效果。

## 兼容性

| 系统版本 | 可用功能 |
| --- | --- |
| ColorOS 15、ColorOS 16 | 磨砂堆叠通知、磨砂控制中心 |
| ColorOS 17 | 仅设置界面和效果演示 |

## 安装与启用

1. 安装 FrostShade 的签名 APK。
2. 在 LSPosed 管理器中启用 FrostShade，并勾选作用域「系统界面」。
3. 重启系统界面，或重启手机。
4. 打开 FrostShade，按需开启「磨砂堆叠通知」和「磨砂控制中心」，并调整外观。

## 从源码构建

准备 JDK 25 和 Android SDK Platform 37.1，在仓库根目录运行以下命令，执行单元测试并构建发布包。

**Windows**

```powershell
.\gradlew.bat :app:testDebugUnitTest :app:assembleRelease
```

**macOS / Linux**

```sh
./gradlew :app:testDebugUnitTest :app:assembleRelease
```

构建产物位于 `app/build/outputs/apk/release/`，签名后即可安装。

## 问题反馈

请在提交问题时附上设备型号、ColorOS 版本及构建号、LSPosed 版本、FrostShade 版本和复现步骤。 [GitHub Issues](https://github.com/MuYuanXing/FrostShade/issues)

## 许可证

FrostShade 的自有源代码采用 [MPL-2.0](https://github.com/MuYuanXing/FrostShade/blob/main/LICENSE)。COUI Kit、Backdrop 和第三方素材沿用各自的许可及权利声明，详见 [NOTICE](https://github.com/MuYuanXing/FrostShade/blob/main/NOTICE)。
