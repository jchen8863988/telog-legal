# TeLog Legal & Support (HTML)

**特档案 TeLog** 独立法律与支持文档库。与 FamilyMedVault 主站产品分离，共用 `familymedvault.com` 域名托管。

## 文件

| 文件 | 用途 | App Store 填写 URL（部署后） |
|------|------|------------------------------|
| `zh/support.html` | 技术支持（中文） | `https://www.familymedvault.com/zh/telog/support` |
| `en/support.html` | Technical Support (EN) | `https://www.familymedvault.com/telog/support` |
| `zh/privacy.html` | **隐私政策（中文）** | `https://www.familymedvault.com/zh/telog/privacy` |
| `en/privacy.html` | **Privacy Policy (EN)** | `https://www.familymedvault.com/telog/privacy` |
| `zh/terms.html` | **用户协议 EULA（中文）** | `https://www.familymedvault.com/zh/telog/terms` |
| `en/terms.html` | **Terms of Use (EN)** | `https://www.familymedvault.com/telog/terms` |
| `index.html` | 默认跳转中文支持页 | — |

GitHub Pages（当前）：`https://jchen8863988.github.io/telog-legal/`

## App Store Connect 填写

| 字段 | 中文区 | 英文区 |
|------|--------|--------|
| **支持网址** | `https://www.familymedvault.com/zh/telog/support` | `https://www.familymedvault.com/telog/support` |
| **隐私政策网址** | `https://www.familymedvault.com/zh/telog/privacy` | `https://www.familymedvault.com/telog/privacy` |
| **EULA / 许可协议** | `https://www.familymedvault.com/zh/telog/terms` | `https://www.familymedvault.com/telog/terms` |
| **联系邮箱** | `telog@familymedvault.com` | 同左 |

GitHub Pages 临时地址：在以上路径将域名换为 `https://jchen8863988.github.io/telog-legal`，文件名加 `.html`（如 `zh/terms.html`）。

## 部署

```bash
mkdir -p "FamilyMedVault web/public/zh/telog" "FamilyMedVault web/public/telog"
cp legal/zh/support.html "FamilyMedVault web/public/zh/telog/support.html"
cp legal/zh/privacy.html  "FamilyMedVault web/public/zh/telog/privacy.html"
cp legal/zh/terms.html   "FamilyMedVault web/public/zh/telog/terms.html"
cp legal/en/support.html "FamilyMedVault web/public/telog/support.html"
cp legal/en/privacy.html  "FamilyMedVault web/public/telog/privacy.html"
cp legal/en/terms.html   "FamilyMedVault web/public/telog/terms.html"
```

## 联系

隐私与支持：`telog@familymedvault.com`
