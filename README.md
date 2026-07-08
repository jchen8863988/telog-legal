# TeLog Legal & Support (HTML)

**特档案 TeLog** 法律与支持文档（独立个人开发者）。版本 **2.0.0**（2026-07-08）按最终产品设计覆盖重写。

## 原则（与 App 一致）

- 面向中国大陆车主合规落地，可同时上架海外；**政策与准据法以中国本地为准**
- 车辆数据仅来自用户**特斯拉官方授权**（Fleet API）
- **默认本机存储**；云端代采 / 备份 / 家庭共享须单独同意
- 联系邮箱统一：**service@telog.cn**
- 含苹果分发所需隐私/EULA/支持页要点，以及**个人开发者免责**表述

## 文件

| 文件 | 用途 | 当前托管 URL（GitHub Pages） |
|------|------|------------------------------|
| `zh/support.html` | 技术支持（中文） | `https://jchen8863988.github.io/telog-legal/zh/support.html` |
| `en/support.html` | Technical Support (EN) | `https://jchen8863988.github.io/telog-legal/en/support.html` |
| `zh/privacy.html` | 隐私政策（中文） | `https://jchen8863988.github.io/telog-legal/zh/privacy.html` |
| `en/privacy.html` | Privacy Policy (EN) | `https://jchen8863988.github.io/telog-legal/en/privacy.html` |
| `zh/terms.html` | 用户协议 EULA（中文） | `https://jchen8863988.github.io/telog-legal/zh/terms.html` |
| `en/terms.html` | Terms of Use (EN) | `https://jchen8863988.github.io/telog-legal/en/terms.html` |
| `zh/cloud-collect-disclosure.html` | 云端代采单独同意说明 | 同仓库 `zh/` |
| `index.html` | 默认跳转中文支持页 | — |

## App Store Connect 填写

| 字段 | 建议值 |
|------|--------|
| **支持网址** | `https://jchen8863988.github.io/telog-legal/zh/support.html`（英文区用 `/en/support.html`） |
| **隐私政策网址** | `https://jchen8863988.github.io/telog-legal/zh/privacy.html`（英文区用 `/en/privacy.html`） |
| **EULA / 许可协议** | `https://jchen8863988.github.io/telog-legal/zh/terms.html`（英文区用 `/en/terms.html`） |
| **联系邮箱** | `service@telog.cn` |

域名正式上线后可将 canonical / Connect 地址改到自有域名，并同步 `src/core/app/appLinks.ts` 中的 `LEGAL_SITE`。

## 部署

见 `DEPLOY.md`。更新后把本目录 `zh/`、`en/` HTML 同步推送到 `telog-legal` 仓库。

## 联系

隐私与支持：`service@telog.cn`
