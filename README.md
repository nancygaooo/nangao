# nancygao.com

Nan Gao 个人主页（单页、中英双语，纯静态，可直接部署到 GitHub Pages）。

## 部署
1. 把本目录全部内容（含隐藏文件 `.nojekyll`）上传到仓库根目录。
2. Settings → Pages → Source 选 `Deploy from a branch`，分支 `main`，目录 `/ (root)`。
3. 继续使用 nancygao.com：在 Pages 设置里填写 Custom domain，再到域名服务商修改 DNS。

## 维护说明
- 所有内容都在 `index.html`，每个版块前有 `<!-- ===== 版块名 ===== -->` 注释。
- 中英文成对书写：`<span class="en">英文</span><span class="zh">中文</span>`。只写一种语言的内容（如论文标题）两种模式下都会显示。
- 新增一条动态：复制 News 版块里的一整行 `<li>…</li>`，改日期和文字。
- 新增论文：复制 Publications 里的一整个 `<li>…</li>`；论文 PDF 放进 `wp-content/uploads/` 后用相对路径链接。
- 保留 `wp-content/uploads/` 原路径，是为了让外部网站指向旧 PDF 的链接继续有效。
- 研究方向：Research 版块一排三列；配图是 `assets/research/1.svg`–`3.svg`，换成自己的图片时改 `<img src>` 即可（建议 4:3 比例）。
- 版块小猫：`assets/cats/` 下每个版块一张 SVG，可单独替换。原 News 猫咪照片仍在 `wp-content/uploads/2022/09/WeChat-Image_20210518205720.png`。
- 链接 `https://nancygao.com/?lang=zh` 可直接打开中文版。
