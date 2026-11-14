# 更新日志索引

本文件不记录具体版本变更——各仓的变更请看对应仓库的 `CHANGELOG.md` 与 Releases 页面。

## 2026-11-14 · 组织 profile 与文档复核

- 依据 `gh repo list codecloud-dev --json name,isFork` 真实清单复核 `profile/README.md`：补全当前活跃自研仓库（moxsh-terminal、moxsh-proot、moxwebgpu、agent-core、mox-id、moxsh-suite、moxsh-plugins、mox-site、molecule-os、molecule-lm、pdf-lib-plus），排除 `awesome-*` fork；补充 npm 组织 `@codecloud-dev` 与官网 mox-site.pages.dev。
- 评估组织级配置：`SECURITY.md`（含私密漏洞报告入口、响应时效）、`CONTRIBUTING.md`（明确不要求 GPG/DCO/CLA）、`CODE_OF_CONDUCT.md`（独立投诉表单）判定为完整，予以保留。
- 评估 `.github/dependabot.yml`：本仓无 `package.json`，仅 `github-actions` 生态有意义，保留现有按月分组 minor/patch、major 走人工的配置。
- 复核 `ISSUE_TEMPLATE/`（bug_report.yml / feature_request.yml / config.yml）中文提示，判定仍适用，未做改动。

| 仓库 | 内容 |
| --- | --- |
| `moxsh-terminal` | Android 终端 App + Rust 终端内核 |
| `moxsh-proot` | PRoot 引擎 + 安装器 |
| `moxwebgpu` | 浏览器 WebGPU 深度学习框架 |
| `agent-core` | AI Agent SDK |
| `moxsh-plugins` | .mox 插件目录与规范 |
| `moxsh-suite` | 全家桶聚合与跨仓规格 |
| `mox-id` / `mox-site` | 身份后端与官网（私有） |
