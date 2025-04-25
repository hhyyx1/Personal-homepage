# 二次元动漫小屋 - 个人主页模板 (Anime House - Personal Homepage Template)

这是一个充满活力的、以动漫/二次元为主题的个人主页 HTML 模板。它利用 Tailwind CSS、自定义 CSS 动画和外部 API 来创建一个视觉上吸引人且动态的单页网站。

![个人主页展示.png](https://cfimg.7374520.xyz/file/1745592695990_个人主页展示.png) 
*(建议在此处添加项目截图)*

## ✨ 主要功能 (Features)

*   **动漫/可爱美学 (Anime/Kawaii Aesthetic):** 整体设计风格偏向可爱、粉色调的二次元风格。
*   **响应式设计 (Responsive Design):** 使用 Tailwind CSS 构建，能适应不同屏幕尺寸（桌面、平板、手机）。
*   **动态背景 (Dynamic Background):** 页面背景使用外部 API 随机加载动漫图片，并设置定时刷新。
*   **随机图片加载 (Random Image Loading):** 页面中多个图片元素（如 Logo、主要角色、作品展示图等）通过添加 `Math.random()` 参数尝试从外部 API  获取随机动漫图片。
*   **图片加载占位符与加载动画 (Image Placeholders & Spinners):** 在图片加载完成前显示占位背景和加载旋转图标，提升用户体验。
*   **樱花飘落动画 (Sakura Falling Animation):** 使用 JavaScript 和 CSS 动画模拟樱花花瓣飘落的效果，增加氛围感。
*   **CSS 动画效果 (CSS Animations):** 包含元素浮动 (`floating`)、弹跳 (`bounce`)、闪烁 (`sparkle`)、霓虹灯文字 (`neon-text`) 等多种 CSS 动画。
*   **交互式悬停效果 (Interactive Hover Effects):** 卡片、角色图片、链接等元素在鼠标悬停时具有缩放、旋转、阴影变化等交互效果。
*   **常见页面结构 (Standard Sections):** 包含导航栏、英雄区域、关于我、作品集、博客精选和页脚等标准个人主页模块。
*   **图标集成 (Icon Integration):** 使用 Font Awesome 提供各种图标。
*   **自定义字体 (Custom Fonts):** 引入并使用了特定的中文字体 (`Ma Shan Zheng`, `ZCOOL KuaiLe`) 以符合主题风格。

## 🛠️ 使用技术 (Technologies Used)

*   **HTML5:** 页面结构。
*   **CSS3:** 基础样式、自定义动画、布局 (Flexbox, Grid)。
*   **Tailwind CSS v3:** 主要的 CSS 框架，用于快速构建响应式布局和样式。
*   **JavaScript (Vanilla JS):** 用于实现樱花飘落动画、动态背景加载和图片加载状态处理。
*   **Font Awesome 6:** 提供矢量图标。
*   **Google Fonts:** 加载自定义网页字体。
*   **外部图片 API:**
    *   `https://www.example.com/api.php?*****=images`
    *   `https://www.example.com/api/file/`
    *(注意：不一定必须是这些格式)*

## 🚀 如何部署 (Deployment)

这是一个纯粹的前端项目（静态网站），不依赖任何后端服务（除了外部图片 API）。因此，它可以轻松部署到任何支持静态文件托管的服务上。

**部署选项包括：**

1.  **GitHub Pages:**
    *   将代码推送到 GitHub 仓库。
    *   在仓库的 `Settings` -> `Pages` 中，选择 `main` (或 `master`) 分支进行部署。
2.  **Netlify:**
    *   将代码推送到 GitHub/GitLab/Bitbucket 仓库。
    *   在 Netlify 上连接该仓库，它会自动构建和部署。
    *   或者直接将 HTML 文件拖放到 Netlify 的部署区域。
3.  **Vercel:**
    *   类似于 Netlify，可以连接 Git 仓库进行自动部署，或直接上传。
4.  **Cloudflare Pages:**
    *   类似于 Netlify/Vercel，连接 Git 仓库进行部署。
5.  **传统虚拟主机/服务器 (Traditional Hosting/Server):**
    *   将 `index.html` 文件（可以将代码保存为此文件名）上传到你的 Web 服务器（如 Apache, Nginx）的网站根目录或指定目录下即可访问。

**部署步骤（通用）：**

1.  将上述 HTML 代码保存为一个 `.html` 文件（例如 `index.html`）。
2.  选择上述任一托管平台。
3.  按照该平台的说明上传或连接你的代码仓库。
4.  完成部署后，你将获得一个公开的 URL 来访问你的网站。

## 📝 注意事项 (Notes)

*   **外部 API 依赖:** 该页面的视觉效果（背景、大部分图片）严重依赖于外部的随机图片 API 。如果这些 API 失效或不稳定，图片将无法加载（尽管代码中包含 `onerror` 处理，但部分 fallback 仍然指向同一 API，可能无法完全解决问题）。为了更稳定的部署，建议将图片资源本地化或使用更可靠的图床/CDN 服务。
*   **性能:** 大量使用外部 API 加载图片可能会影响页面加载速度和性能。
*   **移动端导航:** 页面中包含一个移动端的汉堡菜单图标 (`<i class="fas fa-bars"></i>`)，但没有实现相应的 JavaScript 来切换导航菜单的显示/隐藏。
*   **链接:** 页面中的大部分链接 (`<a>` 标签) 都指向 `example.com` 或 `#`，需要根据实际需求修改为有效的目标地址。

---
