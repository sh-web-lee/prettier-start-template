# 🎨 前端代码规范统一配置

> 开箱即用的 ESLint + Prettier + Husky 集成方案，让你告别繁琐配置，专注于业务开发。

---
## ✨ 特性

- **⚡ 开箱即用**：无需手动配置 ESLint 规则、Prettier 选项或 Git 钩子，安装即可生效。
- **🚀 零配置 Prettier**：内置业界通用的代码格式化规则（单引号、尾随逗号、2 空格等），直接使用。
- **🪝 提交前自动美化**：基于 Husky 和 lint-staged，在 `git commit` 时自动格式化暂存区代码，确保仓库代码风格统一。
- **👥 团队协作友好**：所有配置文件可提交至仓库，新成员克隆后 `npm install` 即可同步规范，消除因环境差异导致的格式冲突。
- **🌐 跨框架支持**：同时支持 **Vue** 和 **React** 项目（通过简单注释切换），也支持 TypeScript。
---
## 🚀 快速开始
### 1. 克隆项目
```bash
git clone git@github.com:sh-web-lee/prettier-start-template.git
```
### 2. 安装依赖（可选）
项目已集成所需依赖，克隆后可直接启动，若依赖缺失，执行以下命令：
```bash
# npm
npm install

# yarn
yarn install

# pnpm
pnpm install
```
### 3. 开始开发
直接编写代码，提交时将自动触发Prettier格式化，无需额外操作。
---
## 📌 功能详情
|功能|说明|使用方式
|开箱即用|无需手动配置Prettier，克隆即开发|克隆项目后直接编写代码
|自动格式化|提交代码前自动执行Prettier，美化代码格式|执行git commit，自动触发格式化
|风格统一|团队共享统一Prettier配置，协同开发无格式冲突|所有成员克隆项目后，自动使用统一配置
|配置可扩展|支持自定义Prettier规则，适配项目特殊需求|修改项目根目录.prettierrc文件即可
---
## ⚙️ 自定义配置（可选）
若项目需要自定义Prettier格式规则，可修改项目根目录下的 .prettierrc 文件，示例配置如下：
```bash
{
  "printWidth": 120,        // 每行代码最大长度
  "tabWidth": 2,            // 缩进宽度
  "useTabs": false,         // 不使用tab缩进，使用空格
  "singleQuote": true,      // 使用单引号
  "semi": true,             // 语句结尾加分号
  "trailingComma": "all",   // 所有对象/数组末尾加逗号
  "bracketSpacing": true,   // 对象括号前后加空格
  "arrowParens": "always"   // 箭头函数参数必须加括号
}
```
更多Prettier配置项，可参考 Prettier官方文档。
---
## 🤝 团队协作说明
1. 所有团队成员克隆项目后，无需额外配置，自动使用统一的Prettier规则。
2. 提交代码时，git hooks会自动执行格式化，若格式化失败，将阻止提交，需修复格式后重新提交。
3. 若需修改格式化规则，需团队协商一致后，修改根目录.prettierrc文件，并提交到仓库，确保所有成员同步更新。
---
## ❓ 常见问题
- Q：提交代码时，自动格式化失败怎么办？
A：检查代码是否有语法错误，修复语法错误后重新提交；若仍失败，可手动执行 npx prettier --write . 手动格式化所有代码，再提交。
- Q：如何关闭自动格式化功能？
A：删除项目根目录下的 .husky 文件夹，即可关闭提交前自动格式化（不推荐）。
- Q：自定义配置后，格式不生效？
A：修改.prettierrc文件后，重启VS Code，或执行 npx prettier --write . 手动触发格式化。
---
## 📞 联系与反馈
若使用过程中遇到问题，或有功能优化建议，可通过以下方式反馈：
- [[项目仓库Issues](https://github.com/sh-web-lee/prettier-start-template/issues)]
- [shwenlee@gmail.com]
---
### 温馨提示
建议所有团队成员在VS Code中安装 Prettier插件，配合本项目使用，可实现实时格式化，提升开发体验。