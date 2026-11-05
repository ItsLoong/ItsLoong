<p align="center">
  <img src="./assets/moonlight-banner.webp" width="100%" alt="Loong 的月夜观测室：银紫发少女与小白龙，窗外是星空与云海" />
</p>

<h1 align="center">月夜观测室</h1>

<p align="center"><b>把灵感写进代码，把世界记录成帧。</b></p>

<p align="center">
  我是 <b>Loong</b>，这里放着我的 C++ 工具与 RGB-D 采集实验。<br />
  欢迎来我的小小观测室坐坐。
</p>

<p align="center">
  <img src="./assets/typing.svg" width="520" alt="C++20 · RGB-D · 开源工具" />
</p>

<p align="center">
  <a href="https://github.com/ItsLoong/ObCapture">ObCapture</a>
  &nbsp; · &nbsp;
  <a href="https://github.com/ItsLoong/ObCapture/tree/main/docs">开发笔记</a>
  &nbsp; · &nbsp;
  <a href="https://github.com/ItsLoong?tab=repositories">全部仓库</a>
</p>

<br />

## 工作台上的小作品

### [ObCapture](https://github.com/ItsLoong/ObCapture)

**让相机看到的世界，成为可以保存、检查与回放的数据。**

基于 Orbbec SDK v2 的现代 C++ 相机采集、录制与诊断库，优先支持 Gemini 338Le 以太网 RGB-D 相机。

<p>
  <img src="./assets/cpp.svg" alt="C++20" />
  <img src="./assets/cmake.svg" alt="CMake" />
  <img src="./assets/rgbd.svg" alt="RGB-D" />
  <img src="./assets/license.svg" alt="ObCapture 使用 MIT 许可证" />
</p>

- **找到设备** — 按序列号或 IP 选择相机，查看可用的数据流配置
- **留下每一帧** — 异步保存图像、IMU 数据与逐帧索引，保留时间戳和深度信息
- **让记录可检查** — 保存会话状态与校验信息，支持脱离相机的离线校验

[查看源码](https://github.com/ItsLoong/ObCapture) · [采集指南](https://github.com/ItsLoong/ObCapture/blob/main/docs/Capture.md) · [回放指南](https://github.com/ItsLoong/ObCapture/blob/main/docs/Playback.md)

<details>
<summary><b>打开工具抽屉：构建与验证</b></summary>

<br />

项目使用 C++20 与 CMake，并提供不依赖相机或 SDK 的核心构建和离线测试路径。

```sh
cmake -S . -B build-offline -DOBCAPTURE_WITH_ORBBEC=OFF
cmake --build build-offline --parallel
ctest --test-dir build-offline --output-on-failure
```

在 ObCapture 仓库根目录执行上述命令。完整依赖与相机构建步骤见 [项目说明](https://github.com/ItsLoong/ObCapture#readme)。

</details>

<br />

<p align="center">
  <img src="./assets/star-divider.svg" width="600" alt="星月分隔线" />
</p>

<p align="center"><sub>谢谢你路过这里。愿下一次灵感，也像星光一样抵达。</sub></p>
