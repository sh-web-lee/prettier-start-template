# 📦 eslint-config & prettier-config

一个开箱即用的 ESLint 与 Prettier 配置集，帮助你快速在新项目中统一代码风格和规范。支持 Vue 和 React 项目，基于最新的 ESLint 9.x 扁平化配置（Flat Config）设计。

## ✨ 特性

✅ 集成 ESLint 推荐规则

✅ 集成 Prettier 规则，自动解决代码格式冲突

✅ 支持 JavaScript / TypeScript

✅ 可选启用 Vue 或 React 插件（通过简单配置）

✅ 提供 .prettierrc.js 通用格式化配置

✅ 零冗余，按需安装依赖

## 📦 安装

在你的项目根目录执行：

```
# 安装核心依赖
npm install -D eslint prettier

# 安装 ESLint 插件和解析器
npm install -D @eslint/js globals

# 如果你使用 TypeScript
npm install -D typescript-eslint

# 如果你使用 Vue
npm install -D eslint-plugin-vue

# 如果你使用 React
npm install -D eslint-plugin-react eslint-plugin-react-hooks
```
