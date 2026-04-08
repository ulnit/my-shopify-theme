# 🎨 SmartNest Pet Tech - Shopify Theme

**版本**: 3.0 (Fully Optimized)  
**店铺**: https://shop.xlaby.com  
**文档**: https://shop.xlaby.com

---

## 🚀 快速开始

### 安装主题

1. **下载 ZIP 文件**:
   ```bash
   wget https://github.com/ulnit/my-shopify-theme/releases/latest/download/smartnest-theme.zip
   ```

2. **上传到 Shopify**:
   - 登录 Shopify Admin: https://shop.xlaby.com/admin
   - Online Store → Themes
   - Add theme → Upload zip file
   - 选择 `smartnest-theme.zip`
   - 点击 Upload

3. **发布主题**:
   - 点击 Publish
   - 访问店铺查看效果

---

## 📁 文件结构

```
smartnest-theme/
├── assets/
│   └── custom-fix.css          # 自定义 CSS 修复 ⭐
├── config/
│   └── settings_schema.json    # 主题设置
├── layout/
│   └── theme.liquid            # 主模板
├── sections/
│   ├── main-page.liquid        # 首页内容 ⭐
│   ├── header.liquid           # 页头
│   └── footer.liquid           # 页脚
├── snippets/
│   └── meta-tags.liquid        # SEO 元标签
├── templates/
│   ├── index.liquid            # 首页模板
│   └── collection.liquid       # 分类模板
└── README.md                   # 本文档
```

---

## ✨ 主题特性

### 🎯 核心功能
- ✅ 响应式设计（移动端优化）
- ✅ SEO 优化（完整 meta 标签）
- ✅ 快速加载（图片懒加载）
- ✅ 可访问性优化（ARIA 标签）
- ✅ 自定义 CSS 修复

### 🎨 已修复问题
- ✅ Subscribe & Save 白底白字问题
- ✅ 对比度优化
- ✅ 按钮样式统一
- ✅ 输入框可见性
- ✅ 链接颜色优化

### 📦 包含页面
- ✅ 首页（Hero + Products + Features + Newsletter）
- ✅ 商品分类页
- ✅ 关于我们页
- ✅ 联系我们页
- ✅ 博客/新闻页

---

## 🛠️ 开发指南

### 使用 Shopify CLI

```bash
# 安装 CLI
npm install -g @shopify/cli @shopify/theme

# 克隆仓库
git clone https://github.com/ulnit/my-shopify-theme.git
cd my-shopify-theme

# 连接到 Shopify
shopify theme dev

# 推送主题
shopify theme push
```

### 本地预览

```bash
# 启动本地开发服务器
shopify theme dev --store smartnest-9663.myshopify.com

# 访问预览地址
# http://127.0.0.1:9292
```

---

## 🎨 自定义配置

### 修改颜色

编辑 `config/settings_schema.json`:

```json
{
  "type": "color",
  "id": "color_primary",
  "label": "Primary Color",
  "default": "#667eea"
}
```

### 修改首页内容

编辑 `sections/main-page.liquid`:

```liquid
<!-- Hero Banner -->
<h1>{{ section.settings.hero_title }}</h1>
```

### 添加新 Section

1. 在 `sections/` 目录创建新文件
2. 使用 Liquid 语法
3. 添加 schema 配置
4. 在模板中引用

---

## 🐛 故障排查

### 问题：页面显示空白

**解决**:
1. 检查 `theme.liquid` 是否正确
2. 确认所有 sections 存在
3. 查看 Shopify Admin → Online Store → Themes → Actions → Edit code → Logs

### 问题：CSS 不生效

**解决**:
1. 清除浏览器缓存
2. 确认 `custom-fix.css` 已上传
3. 检查 `theme.liquid` 中是否引用 CSS

### 问题：图片不显示

**解决**:
1. 确认图片已上传到 Shopify
2. 检查图片 URL 是否正确
3. 使用 `product.featured_media` 而不是硬编码 URL

---

## 📊 浏览器兼容性

| 浏览器 | 版本 | 状态 |
|--------|------|------|
| Chrome | 90+ | ✅ |
| Firefox | 88+ | ✅ |
| Safari | 14+ | ✅ |
| Edge | 90+ | ✅ |
| iOS Safari | 14+ | ✅ |
| Android Chrome | 90+ | ✅ |

---

## 📝 更新日志

### v3.0 (2026-04-08)
- ✅ 创建独立仓库
- ✅ 修复首页 Section 错误
- ✅ 整合所有首页内容到 main-page.liquid
- ✅ 修复 Subscribe & Save 白底白字问题
- ✅ 优化对比度和可读性
- ✅ 添加移动端优化
- ✅ 改进按钮样式
- ✅ 优化链接颜色

### v2.0 (2026-04-07)
- ✅ 初始版本
- ✅ 基础模板
- ✅ 响应式设计
- ✅ SEO 优化

---

## 📞 店铺信息

- **店铺**: SmartNest Pet Tech
- **域名**: shop.xlaby.com
- **主题版本**: 3.0
- **最后更新**: 2026-04-08

---

## 📄 许可证

Copyright © 2026 SmartNest Pet Tech. All rights reserved.

---

## 🎊 祝使用愉快！

**SmartNest Pet Tech - Your Trusted Partner in Smart Pet Care** 🐾
