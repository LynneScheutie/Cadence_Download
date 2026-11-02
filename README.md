<div align="center">

# Cadence

4K 目押音游，桌面版。S / D / J / K 四键，五档难度，带演示模式、暂停与计分。

**macOS 与 Windows 都能直接跑，不用开浏览器**

**本仓库只放安装包，源代码在 [Cadence](https://github.com/LynneScheutie/Cadence)。**

</div>

---

## 下载

| 平台 | 文件 | 大小 | 怎么用 |
| --- | --- | --- | --- |
| macOS（Apple 芯片） | [Cadence-1.2.0-arm64.dmg](../../releases) | 117 MB | 打开 dmg，把 Cadence 拖进「应用程序」 |
| macOS（Intel） | [Cadence-1.2.0.dmg](../../releases) | 120 MB | 同上 |
| Windows（x64） | [Cadence-1.2.0-win.zip](../../releases) | 146 MB | 解压后直接运行 `Cadence.exe`，绿色免安装 |
| Windows（ARM） | [Cadence-1.2.0-arm64-win.zip](../../releases) | 144 MB | 同上 |

## 安装

两个平台都没有做代码签名。

- **macOS**：首次打开若提示「无法验证开发者」，到「系统设置 → 隐私与安全性」点「仍要打开」。如果提示文件已损坏，终端执行：

```bash
xattr -dr com.apple.quarantine /Applications/Cadence.app
```

- **Windows**：若被 SmartScreen 拦一下，点「更多信息 → 仍要运行」即可。zip 解压到任意目录就能用，不写注册表。

## 操作

| 按键 | 功能 |
| --- | --- |
| S / D / J / K | 四条轨道的判定键 |
| 空格 | 暂停后继续 |
| ESC | 局内暂停，暂停时再按返回主菜单 |

## 这是什么

一个 4K 下落式音游，最初是一次「音乐游戏 + LLM」作业的产物。游戏本体是纯前端实现，不联网，所有判定都在本地算。开发过程、每一代改了什么、以及两次来自学长学姐的关键意见，都写在[源码仓库的 README](https://github.com/LynneScheutie/Cadence) 里。

## 已知局限

- **只有四键**。S / D / J / K 固定映射四条轨道，不支持自定义键位。
- **没有内置曲目**。音符由程序按难度生成，不做谱面导入，也没有音轨。
- **没做签名与公证**，所以首次打开需要手动放行一次。
- 演示模式目前只在默认参数下能稳定跑到理论值。

## 问题反馈

在 [Issues](../../issues) 里提，说明系统版本、Cadence 版本，以及具体在玩哪首、什么操作下出的问题。
