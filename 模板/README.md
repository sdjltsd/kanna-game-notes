# 📖 博客模板使用指南

本模板用于将 Markdown/HTML 内容转换为美观的博客页面。

## 🚀 快速开始

### 1. 复制模板
复制 `blog-template.html` 文件，重命名为你的文章名（如 `我的攻略.html`）

### 2. 修改内容

#### 修改标题和描述
```html
<meta name="description" content="我的描述">
<title>我的标题</title>
```

#### 修改顶部导航标题
```html
<span>我的文章标题</span>  <!-- 顶部导航 -->
<span>文章标题</span>      <!-- 侧边栏标题 -->
```

#### 修改侧边栏目录
找到侧边栏部分，修改链接：
```html
<a href="#overview" class="sidebar-link">🏠 首页</a>
<a href="#section1" class="sidebar-link">📖 第一章</a>
```

#### 修改内容区域
在 `<!-- 内容区域 -->` 下方添加你的内容

#### 修改底部目录
找到 `<nav class="toc">` 部分，添加对应的目录链接

### 3. 添加锚点 ID
为每个章节的 `h2` 或 `h3` 添加 `id` 属性：
```html
<h2 id="chapter1">第一章</h2>
<h3 id="section1-1">第一章第一节</h3>
```

## 📝 内容格式示例

### 引用块
```html
<blockquote>
  <p>这里是引用内容...</p>
</blockquote>
```

### 表格
```html
<table>
  <thead>
    <tr><th>表头1</th><th>表头2</th></tr>
  </thead>
  <tbody>
    <tr><td>内容1</td><td>内容2</td></tr>
  </tbody>
</table>
```

### 技巧卡片
```html
<div class="tips-grid">
  <div class="tip-card">
    <p><strong>💡 技巧名称</strong></p>
    <p>技巧说明...</p>
  </div>
</div>
```

### 章节卡片
```html
<div class="section-card" id="my-section">
  <h3>📖 章节标题</h3>
  <p>章节内容...</p>
</div>
```

## 🎨 Emoji 图标推荐

| 类型 | Emoji | 用途 |
|------|-------|------|
| 导航 | 📖🏠📚⚔️ | 章节、首页、目录 |
| 操作 | ⚖️🔍💡💬 | 法庭、侦探、提示、对话 |
| 物品 | 📦🔑💎🎯 | 道具、钥匙、宝石、目标 |
| 状态 | ⚠️🎉✅❌ | 警告、完成、成功、错误 |
| 人物 | 🧑‍🤝‍🧑👤👥 | 角色、单人、群体 |

## 🔗 发布到 Netlify

### 方法一：手动部署
1. 将修改好的 `.html` 文件上传到 GitHub 仓库
2. Netlify 会自动检测并部署

### 方法二：Obsidian Friday 插件
1. 安装并配置 Friday 插件
2. 配置 Netlify Personal Access Token 和 Site ID
3. 在 Obsidian 中点击发布按钮

## 📱 主题切换

页面右上角有 🌙/☀️ 按钮，点击可切换亮色/暗色主题，主题偏好会自动保存。

## 📁 文件结构

```
个人博客/
├── 模板/
│   └── blog-template.html    # HTML模板
│   └── README.md             # 使用指南（本文件）
├── 游戏攻略/
│   └── 我的攻略.html          # 使用模板创建的文章
└── ...
```

## ⚠️ 注意事项

1. **ID 唯一性**：每个 `id` 值只能出现一次
2. **侧边栏同步**：添加新章节时，记得同步更新侧边栏和底部目录
3. **图片路径**：如果使用本地图片，需要将图片一起上传

---

模板版本：v1.0
最后更新：2026-04-28
