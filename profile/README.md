# Yuxino Labs

<p align="center">
  <strong>个人产品、桌面工具，以及把它们稳定发布出去的基础设施。</strong>
</p>

<p align="center">
  <a href="https://github.com/yuxino/mimi">mimi</a>
  ·
  <a href="https://github.com/yuxino/kiri">kiri</a>
  ·
  <a href="https://github.com/yuxino/koe">Koe</a>
  ·
  <a href="https://github.com/yuxino/koma">Koma</a>
  ·
  <a href="https://github.com/yuxino/satori">Satori</a>
  ·
  <a href="https://github.com/yuxino/tick">Tick</a>
  ·
  <a href="https://ashita.yuxino.cn">Ashita</a>
</p>

---

## 这里是什么

Yuxino Labs 是 [yuxino](https://github.com/yuxino) 开发个人产品、维护产品站点和管理发布链路的工作区。

公开应用的源码与下载通常放在 `yuxino`；产品站点、服务端和内部发布工具集中在这里。组织内大多数仓库目前为私有，下面的「公开项目」和产品站点可以直接访问，内部项目名则作为成员工作区索引。

## 公开项目

| 项目 | 正在做什么 |
| --- | --- |
| [`mimi`](https://github.com/yuxino/mimi) | 把 Mac 或 PC 正在播放的声音变成实时字幕，并按需翻译成中文、英文或日文 |
| [`kiri`](https://github.com/yuxino/kiri) | 本地优先的截图、标注、OCR、区域录屏与素材库，支持 macOS 和 Windows |
| [`Koe`](https://github.com/yuxino/koe) | 为 Apple Silicon Mac 上的 Chromium 视频生成与播放进度同步的本地优先字幕，使用 Whisper `large-v3`，并支持标签页音频回退和可选翻译 |
| [`Koma`](https://github.com/yuxino/koma) | 把视频或视频链接整理成摘要、章节、字幕、关键帧和结构化数据，并汇总在可跳转的时间线上 |
| [`Satori`](https://github.com/yuxino/satori) | 以阅读为中心的 macOS PDF 教材阅读器，可围绕段落、图片和代码块向 AI 提问 |
| [`Tick`](https://github.com/yuxino/tick) | 把 macOS LaunchAgent 定时任务的创建、运行、调试和日志查看做成可视化应用 |
| [Ashita](https://ashita.yuxino.cn) | 记录软件、项目取舍和不想忘掉的事情的双语个人博客 |

<details>
<summary><strong>内部工作区（仅成员可见）</strong></summary>

### 产品与站点

源仓库仅组织成员可见；已经公开的产品站点直接链接到线上地址。

| 项目 | 作用 |
| --- | --- |
| `x` · `x-server` | 个人支出与物品日均成本账本 |
| `comet` · `comet-api` | 看板、卡片和沉浸模式组成的个人任务管理器 |
| `yomi` · `yomi-api` | 可执行单节点或整条流程的可视化工作流编辑器 |
| `paw` · `paw-api` | 像普通文件管理器一样浏览和管理对象存储 |
| `nichijou` · `nichijou-api` | 用动态流、搜索和「那年今日」保存日常记录 |
| `ele` · `ele-api` | 用照片、备注和评分回看每一餐 |
| `ashita` | [Ashita](https://ashita.yuxino.cn) 的内容与站点源码 |
| `home` | [`yuxino.cn`](https://yuxino.cn) 的个人首页与项目入口 |
| `mimi-web` | [mimi 产品官网](https://mimi-web.yuxino.cn) |
| `kiri-web` | [kiri 产品官网](https://kiri-web.yuxino.cn) |

### 发布主链路

| 项目 | 作用 |
| --- | --- |
| `meow` | 个人使用的前端发布控制台，管理项目、构建、版本、预览、灰度、上线和回滚 |
| `meow-api` | Meow 的控制面与站点运行时，管理项目和版本，并把请求路由到对应的 OSS 产物 |
| `meow-release` | 统一 GitHub Action，上传构建产物并回写 `reserve / fail-pending / release` 状态 |
| `meow-bootstrap` | 项目出生器，创建 Vite+ 或 Slidev 仓库并自动接入发布流程 |

这套链路现在可以：

- 创建项目，配置域名、运行方式和构建脚本
- 主动触发构建，并按 GitHub Actions 的精确 Run ID 跟踪结果
- 为每次构建保留独立版本，先预览，再按条件灰度、全量发布或回滚
- 让前端项目共享同一套发布协议，不再各自维护上传脚本

### 模板与共享基础设施

| 项目 | 作用 |
| --- | --- |
| `web-template` | React / Vite 前端项目模板 |
| `server-template` | TypeScript / Express 服务端项目模板 |
| `auth` | 鉴权页与访问入口 |
| `404` | 统一 404 页面 |

</details>

---

<p align="center">
  做自己真的会用，也愿意继续维护的东西。
</p>
