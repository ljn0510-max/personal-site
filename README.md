# 个人简历网站

这是一个个人展示网页模板，用于投递简历和寻找工作机会。

## 目录结构

```
personal-site/
├── index.html          # 主页
├── capabilities.html   # 能力体系入口页（可选）
├── prompt-engineering.html  # Prompt Engineering 详情
├── rag.html           # RAG 详情
├── agent.html         # Agent 详情
├── skills.html        # Skills 详情
├── assets/            # 静态资源目录
│   └── avatar.jpg     # 头像图片
├── resume.pdf         # PDF 简历文件
└── README.md          # 本文件
```

## 快速开始

### 1. 修改个人信息

编辑 `index.html` 文件，替换以下内容：

- **姓名与职位**: ~500-502 行
- **简介**: ~518 行
- **技能栈**: ~523-531 行
- **教育背景**: ~534-536 行
- **工作经历**: ~547-563 行
- **项目作品**: ~575-615 行
- **联系方式**: ~625-638 行

### 2. 编辑能力体系详情页

四个能力子页面分别对应：

| 页面 | 用途 | 编辑位置 |
|------|------|---------|
| `prompt-engineering.html` | 提示词工程实践 | ~90-120 行（概述）、~122-147 行（案例卡片） |
| `rag.html` | RAG 系统构建 | ~90-120 行（概述）、~122-147 行（案例卡片） |
| `agent.html` | 智能体开发 | ~90-120 行（概述）、~122-147 行（案例卡片） |
| `skills.html` | 技术栈展示 | ~120-180 行（技能分类） |

每个页面的**概述部分**有占位符文本，用括号标注，方便查找替换。

### 3. 替换头像

将你的头像图片命名为 `avatar.jpg`，放到 `assets/` 目录下。

### 4. 添加 PDF 简历

将你的 PDF 简历命名为 `resume.pdf`，放在项目根目录。

### 5. 部署到 GitHub Pages

```bash
# 初始化 git 仓库（如果还未初始化）
git init

# 添加所有文件
git add .

# 提交
git commit -m "Add personal portfolio site"

# 创建远程仓库（在 GitHub 上创建后）
git remote add origin https://github.com/你的用户名/personal-site.git
git push -u origin main

# 在 GitHub 设置中开启 Pages
# Settings -> Pages -> Source -> main branch
```

访问地址：`https://你的用户名.github.io/personal-site/`

## 后期维护

- **修改内容**: 直接用文本编辑器或 VS Code 打开对应 HTML 文件修改
- **添加新能力**: 复制现有子页面模板，修改内容和链接即可
- **更换配色**: 修改 `<style>` 标签中的 CSS 变量

## 自定义 CSS 配色

在 `<style>` 开头找到 `:root`，修改颜色值：

```css
:root {
    --primary-color: #2563eb;      /* 主色调 */
    --secondary-color: #1e40af;    /* 次要色调 */
}
```
