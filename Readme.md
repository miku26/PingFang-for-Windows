# Windows 字体替换：PingFang SC & SF Pro Text

一个用于在 Windows 10/11 上替换系统界面字体的个人配置项目。  
目标是将部分系统字体替换为：

- 中文界面：`PingFang SC` / 苹方
- 英文界面：`SF Pro Text`

---

## ⚠️ 重要声明

- `PingFang`、`SF Pro` 等字体版权归 Apple Inc. 所有
- 在非 Apple 设备上使用这些字体可能违反许可协议，请自行评估风险
- 替换系统字体有风险，在操作前请做好备份

---

## 特性

- 将 Windows 中文部分替换为苹方
- 将 Windows 英数部分替换为 SF Pro Text

---

## 应用字体替换

1. 备份原 **Segoe UI、msyh、SegUIVar** 等16个字体。
2. 放在文件夹 **fonts**，**fonts** 为自定义文件夹，确认文件夹位置
3. 找到高级启动，使用命令面板，**Xcopy c:/fonts c:/windows/fonts**

重启系统。

---

## 恢复默认字体

方法与替换方法如出一辙

## 存在问题

### PingFang.ttc

目前锁屏界面的汉字、设置界面的部分汉字，如 **“所有功能尽在 Microsoft 账户”** 等，并未落回修改后的微软雅黑

猜测：【1】由 **SegUIVar + 中文字体** 组成的，目前不清楚是由哪个字体控制；【2】可能PingFang.ttc缺少字符导致不显示

PingFang.ttc并未包含 **Bold** 字重，通过线性加粗而来

### PingFangUI.ttc

目前苹果使用的可变字体，字重支持 **UltraLight - Heavy (100-900)**，真正意义上的 **粗体**，同时可能是UI字体的缘故，界面字体统一

PingFangUI.ttc 没有日文字符，会导致日文回退为宋体；同时PingFangUI.ttc能用于替换微软雅黑的就三3个字重 **UltraLight、Medium、Heavy**，界面字体会显得粗

## 免责声明

本项目仅供个人学习、研究和测试使用。 
请勿用于商业分发、盗版传播或任何侵犯字体版权的行为。 
使用前请自行备份系统，并确认你拥有相关字体的合法使用权