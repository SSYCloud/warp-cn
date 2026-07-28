<p align="center">
  <img width="512" alt="WarpCn - 中文汉化版 Warp 终端" src="https://storage.googleapis.com/warpdotdev-content/Readme.png" />
</p>

<h1 align="center">WarpCn — Warp 终端中文汉化版</h1>

<p align="center">
  <a href="https://github.com/SSYCloud/warp-cn/releases">下载</a>
  ·
  <a href="https://www.shengsuanyun.com">胜算云</a>
  ·
  <a href="https://github.com/warpdotdev/Warp">原版 Warp</a>
  ·
  <a href="https://docs.warp.dev">Warp 文档</a>
</p>

<p align="center">
  <a href="https://github.com/SSYCloud/warp-cn/releases"><img alt="GitHub Release" src="https://img.shields.io/github/v/release/SSYCloud/warp-cn?style=flat-square" /></a>
  <a href="LICENSE-AGPL"><img alt="License: AGPL-3.0" src="https://img.shields.io/badge/license-AGPL--3.0-blue?style=flat-square" /></a>
  <a href="https://github.com/warpdotdev/Warp"><img alt="Based on Warp" src="https://img.shields.io/badge/based%20on-Warp-orange?style=flat-square" /></a>
</p>

<h1></h1>

## 项目简介

**WarpCn** 是基于 [Warp](https://github.com/warpdotdev/Warp) 开源终端的中文汉化版本，由胜算云精益开发者社区维护。

[Warp](https://www.warp.dev) 是一款面向开发者的现代化终端，诞生于终端，却不局限于终端。它将传统终端带入了 21 世纪，提供了现代化的 UI 和代码编辑体验，并内置 AI 智能体（Agent）支持。你可以使用 Warp 内置的 Oz 智能体，也可以运行 Claude Code、Codex、Gemini CLI 等 CLI 编码智能体。

WarpCn 的目标是将这款优秀的终端工具完整地带给中文开发者社区，让中文环境下的开发者能够零障碍地使用 Warp 的所有功能。

### 主要改动

- **全量中文汉化**：界面文字、设置页面、提示信息、帮助文档等全部翻译为中文
- **Agent 模型自由**：集成 [胜算云](https://www.shengsuanyun.com/?from=CH_TN1OOJ95) 300+大模型服务开箱即用，同时支持openai兼容接口
- **去除登录门控**：无需 Warp 账号即可使用全部主要功能
- **支持 macOS 和 Windows**：提供 DMG（macOS）和 EXE（Windows）安装包

## 下载安装

从 [GitHub Releases](https://github.com/SSYCloud/warp-cn/releases) 下载最新版本：

| 平台 | 安装包 |
|------|--------|
| macOS (Apple Silicon / Intel) | `.dmg` |
| Windows | `.exe` |

## 关于胜算云与精益开发者社区

<img width="1942" height="809" alt="cf55eeff4fc238e86d16ce39be3502a8" src="https://github.com/user-attachments/assets/b3ed269d-0125-4664-b150-0ba06b52f786" />

胜算云是AI自动生产超级工厂，长三角国家技术创新中心重大扶持项目，打造工业级 AI 任务执行矩阵。依托完整的全球API算力供应链与弹性算力容器，实现云端快速并发执行 AI 任务，持久化工作流编排，矩阵式执行，共享知识库，高效低成本获得可靠计算结果。点击[此处查看](https://watch.shengsuanyun.com/status/shengsuanyun)网关实时稳定性监控。[点击此处](https://www.shengsuanyun.com/?from=CH_TN1OOJ95) 进入模型网关超市获取API算力，注册新用户可获10元模力及首充10%赠送。

精益社区是AIGC和OPC时代的"精益算力"与"工程化落地"实践交流基地。
欢迎加入精益社区！在这里获取Token词元 Router 最佳实践、批处理、云端智能体军团、自动化编码工作流与 OPC 超级个体等实战指南。进群可查看群公告领取精益社区专属10元模力。

<p align="center">
  <img src="http://pinfans-tec.oss-cn-shanghai.aliyuncs.com/lean/20260728-100815.png" width="500" alt="开发者交流群">
</p>

## 从源码构建

```bash
./script/bootstrap   # 平台依赖安装
./script/run         # 编译并运行 WarpCn
./script/presubmit   # 代码格式化、clippy 检查和测试
```

详细的工程指南请参阅 [WARP.md](WARP.md)。


## 与原版 Warp 的关系

| | Warp（原版） | WarpCn（汉化版） |
|---|---|---|
| 源码 | [warpdotdev/Warp](https://github.com/warpdotdev/Warp) | [SSYCloud/warp-cn](https://github.com/SSYCloud/warp-cn) |
| 界面语言 | 英文 | 中文 |
| Agent模型 | OpenAI / Anthropic 等 | openai兼容接口及胜算云|
| 登录要求 | 需要 Warp 账号 | 无需登录 |
| 协议 | AGPL-3.0 | AGPL-3.0 |

WarpCn 基于 Warp 开源代码库（AGPL-3.0 协议）进行二次开发和汉化，遵循 AGPL-3.0 协议的要求开放全部修改的源代码。我们对 Warp 原版团队的开源贡献表示感谢。

## 许可证

Warp 的 UI 框架（`warpui_core` 和 `warpui` crate）遵循 [MIT 协议](LICENSE-MIT)。

本仓库其余代码（包括 WarpCn 的汉化改动）遵循 [AGPL v3 协议](LICENSE-AGPL)。

## 开源依赖

Warp 的诞生离不开以下优秀的开源项目：

* [Tokio](https://github.com/tokio-rs/tokio)
* [NuShell](https://github.com/nushell/nushell)
* [Fig Completion Specs](https://github.com/withfig/autocomplete)
* [Warp Server Framework](https://github.com/seanmonstar/warp)
* [Alacritty](https://github.com/alacritty/alacritty)
* [Hyper HTTP library](https://github.com/hyperium/hyper)
* [FontKit](https://github.com/servo/font-kit)
* [Core-foundation](https://github.com/servo/core-foundation-rs)
* [Smol](https://github.com/smol-rs/smol)

## 反馈与贡献

- 提交 Issue：[GitHub Issues](https://github.com/SSYCloud/warp-cn/issues)
- 胜算云官网：[https://www.shengsuanyun.com](https://www.shengsuanyun.com)
- 原版 Warp 问题：[warpdotdev/Warp Issues](https://github.com/warpdotdev/Warp/issues)
