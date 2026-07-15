# MyBlog 项目长期记忆

## 项目概述
- **仓库**: https://github.com/Gavinzll/blog.git
- **模板**: AstroPaper v6.1.0 (Astro 7 + Tailwind CSS 4 + TypeScript)
- **本地路径**: /Users/gavin/WorkBuddy/myBlog
- **GitHub 用户名**: Gavinzll
- **Git 凭据**: 已通过 `git credential approve` 存储到系统凭据库，push/pull 无需手动输入 token

## 技术栈
- Astro 7 (静态站点生成)
- Tailwind CSS 4 (样式)
- MDX 支持 (富文本文章)
- Pagefind (静态搜索)
- Satori (动态 OG 图片生成)
- pnpm (包管理)
- Node >= 22.12.0

## 关键文件
- `astro-paper.config.ts` — 站点核心配置（标题、描述、作者、社交链接、功能开关）
- `astro.config.ts` — Astro 构建配置（集成、Markdown、字体等）
- `src/styles/theme.css` — 主题配色变量（亮色/暗色）
- `src/content/posts/` — 博客文章目录
- `src/content/pages/about.md` — 关于页面内容
- `src/pages/index.astro` — 首页（hero 区域文案需自定义）

## 当前状态
- 模板已克隆，依赖已安装，开发服务器可正常启动 (localhost:4321)
- **已个性化**：站点标题 "Gavin's Blog"，作者 "Gavin"，首页 hero 个人问候，关于页面
- GitHub PAT 已安全存储到 `~/.git-credentials`（credential.helper=store），push/pull 无需手动输入
- **GitHub Pages 已配置完成并上线**：https://gavinzll.github.io/blog/
- 部署方式：GitHub Actions（`.github/workflows/deploy.yml`），push 到 main 自动触发构建部署
- site URL 已设为 `https://gavinzll.github.io/blog/`，base 路径已设为 `/blog/`
- 导航栏：Posts, Tags, About, Portfolio, Search（已移除 Archives）
- 社交链接：GitHub (github.com/Gavinzll) + 邮箱 (gavenaazll@gmail.com)
- Portfolio 链接指向 GitHub profile（需用户更新为实际作品集 URL）
- 时区：Asia/Shanghai
- **配色方案**：匹配 satnaing.dev/blog 风格 — 亮色 teal accent (#007a7a)，暗色 mint green accent (#05ce91)
- **首页金句**：每次刷新随机显示一条中文金句（20 条：经典诗词 + 程序员名言 + 名人语录混合）
- **中文字体**：霞鹜文楷 (LXGW WenKai)，通过 CDN 加载，已集成到全局字体栈
  - 字体栈: `Google Sans Code, LXGW WenKai, PingFang SC, Microsoft YaHei, sans-serif`
  - 英文字符使用 Google Sans Code，中文字符自动回退到 LXGW WenKai

## 用户偏好
- 显示名：Gavin
- 博客定位：个人综合（技术 + 生活 + 项目分享）
- 社交：GitHub (github.com/Gavinzll) + 邮箱 (gavenaazll@gmail.com)
- 导航风格：精简 + Portfolio
- 配色偏好：喜欢 satnaing.dev/blog 的 teal/mint green 配色
- 邮箱：gavenaazll@gmail.com

## 注意事项
- 用户提供的 GitHub PAT 已安全存储到 git credential，**不要再在任何文件中明文写入 token**
- 开发服务器启动命令: `pnpm dev` (端口 4321)
- 构建命令: `pnpm build`
- 文章格式: Markdown/MDX，frontmatter 包含 author, pubDatetime, title, slug, featured, draft, tags, description
