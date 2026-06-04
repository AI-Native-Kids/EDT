# Vibe Coding 学习产品 · 战略评估报告

一份以**麦肯锡标准**撰写的商业战略评估，分析「用免费学习资源卖 Token」这一新产品 idea —— 以单页 GitHub Pages 网站形式输出，方便分享给合伙人。

> 核心结论：模式成立，但变现逻辑必须从「卖 Token」升级为「卖被 Token 驱动的价值」。

## 📄 报告内容

报告位于 [`docs/index.html`](docs/index.html)，采用金字塔结构（答案先行）、MECE 拆解、情景测算与红队证伪，包含 11 个章节与 10 张图表（Exhibit）：

| # | 章节 | 关键产出 |
|---|------|---------|
| 01 | 执行摘要 | 一句话结论 + 3 大杠杆 + 5 个关键判断 |
| 02 | 市场机会 | 「为什么是现在」两条曲线交汇 |
| 03 | 商业模式解构 | 剃须刀+刀片模型；3 种 Token 变现路径 |
| 04 | 单位经济学 | LTV:CAC 测算、收入幂律、敏感性分析（核心） |
| 05 | 竞争格局 | 定位地图 + 6 个对手画像 |
| 06 | SWOT | 优势 / 劣势 / 机会 / 威胁 |
| 07 | 风险与红队 | 风险矩阵 + 最尖锐的证伪一问 |
| 08 | 战略选项 | 3 条路径，推荐「垂直闭环」 |
| 09 | 落地路线图 | 12 个月、含 180 天 Go/No-Go |
| 10 | 财务情景 | Bear / Base / Bull 三情景 |
| 11 | 数据资产与退出 | 三层变现栈、数据即终极资产、并购退出（不上市） |
| 12 | 附录 | 关键假设清单 + 给合伙人的决策问题 |

> ⚠️ 报告中所有数值均为**示意性假设（illustrative）**，用于揭示商业逻辑与敏感变量，非财务预测。正式决策前须以一手调研与试点数据校验。

## 🚀 发布到 GitHub Pages（约 1 分钟）

1. 把本仓库推送到 GitHub：
   ```bash
   git add .
   git commit -m "Add Vibe Coding strategy assessment report"
   git push
   ```
2. 打开仓库 **Settings → Pages**。
3. 在 **Build and deployment → Source** 选择 **Deploy from a branch**。
4. **Branch** 选择 `main`，文件夹选择 **`/docs`**，点 **Save**。
5. 等待约 1 分钟，访问：`https://<你的用户名>.github.io/<仓库名>/`

## 👀 本地预览

直接用浏览器打开 `docs/index.html` 即可；或起一个本地服务器：

```bash
# Python
python -m http.server 8000 --directory docs
# 然后访问 http://localhost:8000
```

## 🛠 技术说明

- 单文件、零构建：HTML + 内联 CSS + Chart.js（CDN）。
- 字体使用 Google Fonts（Noto Serif/Sans SC），离线时自动回退系统字体。
- 响应式布局，支持打印（可另存为 PDF 发给合伙人）。
