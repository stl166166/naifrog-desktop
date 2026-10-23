# 奶蛙桌宠 · 绷住

Windows 奶蛙桌宠 **v1.3.6**，Electron + TypeScript + Canvas 2D。免安装、免密钥，离线使用。

## 下载 EXE

**[点击下载 Windows x64 免安装程序](https://github.com/stl166166/naifrog-desktop/releases/download/v1.3.6/naifrog-1.3.6-windows-x64.exe)**

- [版本发布页](https://github.com/stl166166/naifrog-desktop/releases/tag/v1.3.6)
- [完整开源源码与运行素材 ZIP](https://github.com/stl166166/naifrog-desktop/releases/download/v1.3.6/naifrog-1.3.6-source.zip)
- [SHA-256 校验文件](https://github.com/stl166166/naifrog-desktop/releases/download/v1.3.6/SHA256SUMS.txt)

先关闭旧版，再双击 EXE 运行，无需安装 Node.js 或 Python。旁边的 **×**、更多玩法和托盘菜单都能退出。本版保留启动后 **30 分钟自动强制退出**，退出后可重新打开。

可将发布页或 EXE 直链发给朋友、豆包等聊天软件。外部软件的收录和下载能力取决于其自身规则。

## 玩法

- 默认惊鸿一瞥；单击播放约 13 秒捧腹大笑，再次点击立即停止。
- 倒地摆手脚，身体留在落点，蓄力后后空翻起跳，落地继续笑 3 秒。
- 2 秒吐出 300 大小分身，随机错开且避让，按空间尽量多放，最多 64 只，一起笑完原地消失。
- 滚轮缩放 64–900，默认高度 300；拖动踏步、奔跑脚步声、撞边形变回弹、三连后空翻。
- 中文更多玩法、静音、音量、大小和位置保存；默认关闭鼠标跟随。

## 开源代码

完整源码和构建所需运行素材在上述 **source.zip** 中。解压进入 `naifrog-desktop`，使用 Node.js 22.12+、pnpm 和 Windows 桌面环境：

```sh
pnpm install --frozen-lockfile
pnpm run build
pnpm exec tsc --noEmit
pnpm test
pnpm start
pnpm run package
```

成品输出到 `release/`。媒体重建方法见源码包内 `docs/ASSETS_REBUILD.md`。

实现代码按 [GPL-3.0](LICENSE) 提供。第三方角色、图片、视频和声音的来源与许可范围见 [THIRD_PARTY.md](THIRD_PARTY.md)、[SOURCES.md](SOURCES.md)；代码许可不扩大第三方素材的授权。源码包不包含激活服务、密钥、私钥或设备绑定记录。

69 项模块检查、96 组布局检查通过。未进行长时间桌宠测试，不宣称长期卡死已彻底解决。
