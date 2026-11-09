# Quill

Han Shen 的个人网站，分享 B2B 营销、数字化与 AI 转型的实践和思考。

本仓库保存 Quill 的静态发布成品。GitHub Pages 从 `main` 分支的根目录提供首页、博客、职业履历和联系页。

计划使用的域名为 `tobmarket.ing`。联系邮箱为 `contact@tobmarket.ing`。

## 更新网站

默认 GitHub Pages 地址使用 `/quill/` 子路径。构建时运行 `NEXT_PUBLIC_BASE_PATH=/quill QUILL_EXPORT_DIR=.quill-pages-export npm run build`，并将 `.quill-pages-export/` 内的文件同步到本仓库根目录。绑定 `tobmarket.ing` 后，运行 `npm run build` 生成域名根路径版本，再同步 `dist/` 内的文件。保留 `.nojekyll`，以及绑定自定义域名后由 GitHub Pages 生成的 `CNAME` 文件。
