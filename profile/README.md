# Yuxino Labs

<p align="center">
  <strong>产品、发布与项目基础设施的统一工作区。</strong>
</p>

<p align="center">
  <a href="https://github.com/yuxino-labs/meow">meow</a>
  ·
  <a href="https://github.com/yuxino-labs/comet">comet</a>
  ·
  <a href="https://github.com/yuxino-labs/yomi">yomi</a>
  ·
  <a href="https://github.com/yuxino-labs/paw">paw</a>
  ·
  <a href="https://github.com/yuxino-labs/nichijou">nichijou</a>
</p>

---

## 我们在做什么

Yuxino Labs 用来集中管理产品仓库、后端服务、内部工具，以及围绕发布和项目初始化的一整套基础设施。

我们偏爱小团队、快速反馈、可维护的基础设施，以及真正天天会被使用的内部工具。

## 当前这条主链路

| 项目 | 作用 |
| --- | --- |
| [`meow`](https://github.com/yuxino-labs/meow) | 发布控制台，管理项目、版本、脚本、主动构建和删除 |
| [`meow-api`](https://github.com/yuxino-labs/meow-api) | 发布运行时、项目元信息、版本切换、删除与 GitHub 编排 API |
| [`meow-release`](https://github.com/yuxino-labs/meow-release) | 统一 GitHub Action，负责 reserve / upload / release |
| [`meow-bootstrap`](https://github.com/yuxino-labs/meow-bootstrap) | 项目出生器，创建新仓库并自动接入 `meow-release` |

这套链路现在已经支持：

- 在 `meow` 里直接创建新项目
- 给项目主动触发构建
- 删除 `meow` 记录、OSS 资源，并可选顺带删 GitHub 仓库
- 统一前端项目发布入口，不再每仓维护一套独立发布脚本

## 前端项目

| 项目 | 说明 |
| --- | --- |
| [`meow`](https://github.com/yuxino-labs/meow) | 发布控制台 |
| [`comet`](https://github.com/yuxino-labs/comet) | 产品前端 |
| [`yomi`](https://github.com/yuxino-labs/yomi) | 产品前端 |
| [`paw`](https://github.com/yuxino-labs/paw) | 产品前端 |
| [`nichijou`](https://github.com/yuxino-labs/nichijou) | 产品前端 |
| [`ashita`](https://github.com/yuxino-labs/ashita) | 产品前端 |
| [`auth`](https://github.com/yuxino-labs/auth) | 鉴权页与访问入口 |
| [`home`](https://github.com/yuxino-labs/home) | 首页或主入口页面 |
| [`index`](https://github.com/yuxino-labs/index) | 入口页 |

## 后端项目

| 项目 | 说明 |
| --- | --- |
| [`meow-api`](https://github.com/yuxino-labs/meow-api) | 发布运行时与管理 API |
| [`comet-api`](https://github.com/yuxino-labs/comet-api) | comet 后端服务 |
| [`yomi-api`](https://github.com/yuxino-labs/yomi-api) | yomi 后端服务 |
| [`paw-api`](https://github.com/yuxino-labs/paw-api) | paw 后端服务 |
| [`nichijou-api`](https://github.com/yuxino-labs/nichijou-api) | nichijou 后端服务 |
| [`x-server`](https://github.com/yuxino-labs/x-server) | 通用服务端项目 |

## 模板与基础设施

| 项目 | 说明 |
| --- | --- |
| [`meow-release`](https://github.com/yuxino-labs/meow-release) | 统一发布入口与 GitHub Action |
| [`meow-bootstrap`](https://github.com/yuxino-labs/meow-bootstrap) | 新项目初始化与接入器 |
| [`web-template`](https://github.com/yuxino-labs/web-template) | 前端项目模板 |
| [`server-template`](https://github.com/yuxino-labs/server-template) | 服务端项目模板 |
| [`404`](https://github.com/yuxino-labs/404) | 通用 404 页面 |
| [`x`](https://github.com/yuxino-labs/x) | 实验或通用项目 |

## 一些偏好

- 先跑通，再持续打磨
- 发布链路尽量可见、可控
- 系统要能解释清楚，也要能自己维护
- 内部工具不是摆设，要做到团队愿意天天用

---

<p align="center">
  做能上线、能维护、也能继续长出来的东西。
</p>
