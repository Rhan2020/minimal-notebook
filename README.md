# 极简笔记本应用

一个基于React的极简在线笔记本应用，支持自动保存、主题切换和笔记关联功能，数据存储在浏览器本地存储中。

## 功能特性

- 📝 极简笔记编辑 - 专注于写作的简洁界面
- 💾 自动保存 - 内容实时保存到本地存储
- 🌗 主题切换 - 支持明亮/暗黑主题
- 🔗 笔记关联 - 可以关联相关笔记
- 📋 链接分享 - 一键复制笔记链接
- 🆕 笔记创建 - 快速创建新笔记

## 技术栈

- 前端: React 18 + TypeScript
- 样式: Tailwind CSS
- 路由: react-router-dom
- 图标: Font Awesome
- 构建: Vite

## 快速开始

### 开发环境

1. 确保已安装Node.js (v18+)
2. 克隆仓库:
   ```bash
   git clone <仓库地址>
   ```
3. 安装依赖:
   ```bash
   npm install
   ```
4. 启动开发服务器:
   ```bash
   npm run dev
   ```
5. 访问 http://localhost:3000

### 生产构建

```bash
npm run build
```

构建产物将生成在 `dist/static` 目录。

## 项目结构

```
├── src
│   ├── App.tsx          # 应用根组件
│   ├── components       # 公共组件
│   ├── hooks            # 自定义Hook
│   ├── lib              # 工具函数和API
│   ├── pages            # 页面组件
│   └── index.css        # 全局样式
├── vite.config.ts       # Vite配置
└── tailwind.config.js   # Tailwind配置
```

## 特色功能使用指南

### 创建新笔记

点击右上角"新建"按钮，可以创建新笔记。系统会自动生成4位随机ID作为路径。

### 关联笔记

1. 点击"关联"按钮
2. 输入要关联的笔记路径或完整URL
3. 确认后两篇笔记将建立双向关联

### 主题切换

点击右上角主题切换按钮，可以在明亮/暗黑主题间切换，设置会自动保存。

## 部署

### Docker部署

```bash
docker-compose up --build
```

应用将在 http://localhost:8080 可用

## 许可证

MIT
