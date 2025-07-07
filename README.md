# Frontend Standard Template

基于 Vue 3 + Vite 的前端标准化工程模板，集成当前主流的开发工具链和最佳实践。

## ✨ 特性

- 🚀 Vue 3 + Vite + TypeScript - 现代前端开发技术栈
- 📦 Pinia - 新一代状态管理方案
- 🌍 Vue I18n - 国际化解决方案
- 🔌 Axios - 基于 Promise 的 HTTP 客户端
- 🎨 Less - CSS 预处理器
- 📝 ESLint + Prettier + Stylelint - 代码规范与格式化
- 🎯 Simple Git Hooks + Commitlint - Git 提交规范

## 🚀 快速开始

### 环境要求

- Node.js >= 18.0.1
- npm >= 9.0.0

### 开发流程

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev

# 构建生产版本
npm run build
```

## 📖 开发指南

### 状态管理

```typescript
import { useCounterStore } from '@/stores';

// 在组件中使用 Pinia store
const counter = useCounterStore();
```

### 国际化

```typescript
import { useI18n } from 'vue-i18n';

// 使用翻译
const { t, locale } = useI18n();
console.log(t('hello'));

// 切换语言
locale.value = 'en-US';
```

### 网络请求

开发环境配置（`.env.development`）：

```
VITE_API_BASE_URL = 'http://api.example.com'
```

## 📝 Git 提交规范

```bash
# 提交格式
type(scope?): subject

# 示例
feat(user): add user login
fix(auth): fix token expired
```

常用类型：
- feat: 新功能
- fix: Bug 修复
- docs: 文档更新
- style: 代码格式调整
- refactor: 代码重构
- perf: 性能优化

## 🔧 代码质量

```bash
# 代码检查
npm run lint

# 代码格式化
npm run format
```
