# 部署到 GitHub Pages（telog-legal）

## 正确目录结构

仓库 **根目录** 必须是下面这样（不是单个无扩展名的 `support` / `privacy` 文件）：

```
telog-legal/
├── .nojekyll
├── index.html
├── zh/
│   ├── support.html
│   ├── privacy.html
│   └── terms.html
└── en/
    ├── support.html
    ├── privacy.html
    └── terms.html
```

## 一键同步（在本机 MyAppFactory 根目录执行）

```bash
LEGAL_SRC="Telog/legal"
REPO_DIR="$HOME/telog-legal"   # 改成你的 telog-legal 克隆路径

rm -rf "$REPO_DIR/zh" "$REPO_DIR/en"
mkdir -p "$REPO_DIR/zh" "$REPO_DIR/en"

cp "$LEGAL_SRC/.nojekyll" "$REPO_DIR/"
cp "$LEGAL_SRC/index.html" "$REPO_DIR/"
cp "$LEGAL_SRC/zh/"*.html "$REPO_DIR/zh/"
cp "$LEGAL_SRC/en/"*.html "$REPO_DIR/en/"

# 删除错误上传的无扩展名文件（若存在）
rm -f "$REPO_DIR/support" "$REPO_DIR/privacy" "$REPO_DIR/EULA"

cd "$REPO_DIR"
git add -A
git commit -m "fix: deploy zh/en HTML structure for GitHub Pages"
git push origin main
```

推送后等 1～2 分钟，访问：

| 页面 | URL |
|------|-----|
| 技术支持（中文） | https://jchen8863988.github.io/telog-legal/zh/support.html |
| 隐私政策（中文） | https://jchen8863988.github.io/telog-legal/zh/privacy.html |
| 用户协议（中文） | https://jchen8863988.github.io/telog-legal/zh/terms.html |
| Support (EN) | https://jchen8863988.github.io/telog-legal/en/support.html |

## 404 原因

若仓库根目录只有名为 `support`、`privacy` 的文件（**无 `.html`、无 `zh/`/`en/` 文件夹**），则 `/en/support.html` 会 404。
