# 个人学术主页

一个现代、美观、响应式的个人学术主页模板，适合研究人员、博士生、教授等展示个人学术成果。

## ✨ 特性

- 📱 **完全响应式设计** - 在所有设备上完美显示（手机、平板、电脑）
- 🎨 **现代化UI设计** - 渐变色彩、平滑动画、优雅排版
- ⚡ **性能优化** - 纯HTML/CSS/JS，无需框架，加载快速
- 🧭 **流畅导航** - 固定导航栏、平滑滚动、返回顶部按钮
- 📊 **完整内容板块** - 涵盖个人介绍、教育、研究、论文、荣誉等
- ♿ **易于定制** - 清晰的代码结构，方便修改

## 📂 文件结构

```
HomePage/
├── index.html      # 主HTML文件
├── styles.css      # 样式表
├── script.js       # JavaScript交互
├── README.md       # 说明文档
└── avatar.jpg      # 个人照片（需自行添加）
```

## 🚀 快速开始

### 1. 基础设置

1. **下载所有文件**到您的项目文件夹
2. **添加个人照片**：将您的照片命名为 `avatar.jpg` 放在根目录
3. **打开 `index.html`** 开始编辑

### 2. 自定义内容

#### 修改个人信息

在 `index.html` 中找到以下位置并替换为您的信息：

```html
<!-- 导航栏名称 -->
<div class="nav-logo">您的姓名</div>

<!-- 主页标题 -->
<h1 class="hero-title">您的姓名 (Your Name)</h1>
<p class="hero-subtitle">您的职位 | 您的单位</p>

<!-- 社交链接 -->
<a href="mailto:your.email@example.com" class="social-link">
```

#### 修改各部分内容

每个部分都有对应的 `section` 标签和 ID：

- `#home` - 主页
- `#about` - 关于我
- `#education` - 教育背景
- `#research` - 研究成果
- `#publications` - 发表论文
- `#honors` - 荣誉奖项
- `#experience` - 工作经历
- `#skills` - 技术专长
- `#hobbies` - 兴趣爱好

### 3. 自定义颜色主题

在 `styles.css` 文件的顶部修改颜色变量：

```css
:root {
    --primary-color: #2563eb;      /* 主色调 */
    --secondary-color: #1e40af;    /* 次要色调 */
    --text-color: #1f2937;         /* 文字颜色 */
    /* ... 更多颜色 */
}
```

推荐配色方案：

- **蓝色科技风**：`--primary-color: #2563eb;`
- **紫色优雅风**：`--primary-color: #7c3aed;`
- **绿色自然风**：`--primary-color: #059669;`
- **橙色活力风**：`--primary-color: #ea580c;`

### 4. 添加研究成果

复制以下模板并修改内容：

```html
<div class="research-card">
    <div class="research-image">
        <img src="您的研究图片.jpg" alt="研究描述">
    </div>
    <div class="research-content">
        <h3>研究成果标题</h3>
        <p class="research-authors"><strong>您的姓名</strong>, 合作者1, 合作者2</p>
        <p class="research-journal">期刊名称, 2024, 卷(期): 页码</p>
        <p class="research-description">研究描述...</p>
        <div class="research-links">
            <a href="#" class="btn-link">论文链接</a>
            <a href="#" class="btn-link">代码</a>
        </div>
    </div>
</div>
```

### 5. 添加发表论文

在相应的列表中添加：

```html
<li>
    <strong>您的姓名</strong>, 合作者1, 合作者2, 等. 
    "论文标题。" 
    <em>期刊名称</em>, 2024, 卷(期): 页码.
    <a href="https://doi.org/xxx" class="pub-link">[链接]</a>
</li>
```

## 🎯 部署到GitHub Pages

### 方法1：通过GitHub网站

1. 在GitHub创建新仓库，命名为 `yourname.github.io`
2. 上传所有文件到仓库
3. 进入仓库 Settings → Pages
4. Source 选择 `main` 分支
5. 访问 `https://yourname.github.io` 查看您的网站

### 方法2：使用Git命令行

```bash
# 初始化Git仓库
git init
git add .
git commit -m "初始化个人主页"

# 连接到GitHub仓库
git remote add origin https://github.com/yourname/yourname.github.io.git

# 推送到GitHub
git branch -M main
git push -u origin main
```

## 📝 内容填写指南

### 关于我部分
- 简要介绍您的当前职位和工作单位
- 说明您的研究方向和主要课题
- 突出重要成就（论文数量、h-index等）

### 教育背景
- 按时间倒序排列（最新的在最上面）
- 包含时间、学位、专业、学校、城市

### 研究成果
- 选择3-5个最重要的研究成果
- 每个包含：图片、标题、作者、期刊、描述、链接
- 用粗体标注您的名字

### 发表论文
- 分类：第一作者、共同第一作者、合作者
- 使用规范的引用格式
- 提供DOI或论文链接

### 荣誉奖项
- 包含获奖时间和奖项名称
- 如有获奖比例，可以注明

### 工作经历
- 包含职位、单位、时间、地点
- 受邀报告单独列出

### 技术专长
- 分类展示：编程语言、工具、框架等
- 只列出您真正掌握的技能

### 兴趣爱好
- 展示个人性格和生活态度
- 可以包含照片或图标

## 🎨 高级定制

### 修改渐变背景

在 `styles.css` 中找到 `.hero` 类：

```css
.hero {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```

推荐渐变色工具：[uiGradients](https://uigradients.com/)

### 添加自定义字体

在 `<head>` 标签中添加Google Fonts：

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@400;500;700&display=swap" rel="stylesheet">
```

然后在CSS中使用：

```css
body {
    font-family: 'Noto Sans SC', sans-serif;
}
```

### 添加动画效果

参考 `script.js` 中的滚动动画代码，可以为更多元素添加动画。

## 📱 浏览器支持

- ✅ Chrome (推荐)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ 移动端浏览器

## ⚠️ 注意事项

1. **图片优化**：使用前请压缩图片，推荐使用 [TinyPNG](https://tinypng.com/)
2. **个人信息**：仔细检查所有联系方式和链接
3. **内容更新**：定期更新您的研究成果和论文
4. **备份**：定期备份您的网站文件

## 💡 常见问题

### 如何更改网站图标？

将您的图标文件命名为 `favicon.ico`，放在根目录，并在 `<head>` 中添加：

```html
<link rel="icon" type="image/x-icon" href="favicon.ico">
```

### 如何添加更多部分？

复制现有的 `<section>` 标签，修改ID和内容，然后在导航栏添加对应链接。

### 网站加载慢怎么办？

1. 压缩所有图片
2. 使用CDN加载Font Awesome
3. 启用浏览器缓存

### 如何添加访问统计？

可以使用Google Analytics或其他统计服务，在 `</body>` 前添加统计代码。

## 📧 需要帮助？

如果您在使用过程中遇到问题，可以：

1. 检查浏览器控制台的错误信息
2. 确保所有文件路径正确
3. 验证HTML/CSS语法

## 📜 许可证

本模板可免费使用和修改。如果您觉得有用，欢迎分享给其他人！

---

**祝您创建出精美的个人主页！** 🎉

如有任何问题或建议，欢迎反馈。

