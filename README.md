# Markdown 流程图渲染器

单文件网页（`index.html`，无需构建）：粘贴 Markdown，实时渲染其中的流程图，并一键复制为 PNG。

- 支持 ```` ```mermaid ```` 代码块、直接粘贴的 Mermaid 代码
- 支持 ASCII 结构图 / 目录树（```` ```text ```` 代码块中含框线字符）
- 每张图可「复制图片」、「下载 PNG」或「下载 SVG」；「复制全部为一张图」会纵向拼接
- 背景：白色 / 透明 / 深色；主题、清晰度（2x–4x）可选
- 「打开 .md」或直接把文件拖进页面
- 点击任意一张图可放大预览：滚轮缩放、拖动平移、双击适应
- 输入内容和设置自动保存在浏览器本地

运行：`python3 -m http.server` 后访问 `http://localhost:8000`（复制到剪贴板需要 HTTPS 或 localhost）。Mermaid 已内置在 `vendor/`，完全离线可用，也可直接双击 `index.html`（但此时无法复制到剪贴板，仍可下载）。

## 在线使用（GitHub Pages）

仓库 Settings → Pages → Source 选 `Deploy from a branch`，分支 `main`、目录 `/ (root)`，保存后访问 `https://attention-ai-yee.github.io/md-flowchart/`。Pages 是 HTTPS，「复制图片」可直接使用。
