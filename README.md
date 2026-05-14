# 校园心理树洞

## 项目简介

本项目是"鸿雁云程·AI创世纪"创新创业大赛参赛作品，是一个基于 Web 的交互式 AI 心理陪伴应用。用户输入 DeepSeek API Key 后，可以与"树洞精灵"进行温暖的心理对话，获得倾听与陪伴。

## 功能特点

- 💝 AI驱动的心理陪伴聊天
- 📚 心理支持资源推荐
- 🔒 严格的隐私保护
- 📱 响应式设计，支持移动端

## 技术栈

- React 18
- TypeScript
- Vite
- DeepSeek API

## 快速开始

### 安装依赖

```bash
npm install
```

### 开发模式

```bash
npm run dev
```

### 构建生产版本

```bash
npm run build
```

## API Key 使用说明

### 使用方式

1. 用户在应用首页输入 DeepSeek API Key
2. 系统验证 API Key 的有效性
3. 验证通过后进入心理树洞聊天界面
4. 用户可以向"树洞精灵"倾诉心事，获得温暖回应

### 验证方式

- 使用 DeepSeek API 的 `/v1/models` 端点进行验证
- 发送 GET 请求，携带 `Authorization: Bearer {apiKey}` 头部
- 验证成功后进入应用，验证失败显示错误提示

### 隐私处理说明

🔒 **重要隐私声明**：

1. **本地处理**：用户输入的 DeepSeek API Key 仅在浏览器本地内存中临时存储，用于当前会话的 API 调用
2. **不收集**：API Key 不会被上传到任何服务器，不会被收集或记录
3. **不存储**：API Key 不会写入本地存储（LocalStorage/SessionStorage）或 Cookie
4. **会话隔离**：关闭浏览器标签页后，API Key 即被清除
5. **仅用于调用**：API Key 仅用于调用 DeepSeek API 服务，不作他用

## 项目结构

```
├── src/
│   ├── components/
│   │   ├── APIKeyForm.tsx    # API Key 输入与验证组件
│   │   └── StoryGenerator.tsx # 心理树洞聊天组件
│   ├── App.tsx               # 主应用组件
│   ├── App.css               # 应用样式
│   ├── main.tsx              # 入口文件
│   └── index.css             # 全局样式
├── index.html
├── package.json
├── tsconfig.json
└── vite.config.ts
```

## 参赛说明

本作品符合大赛要求：
- ✅ 集成 DeepSeek API
- ✅ API Key 仅用于当前会话，不收集存储
- ✅ 提供 API Key 使用方式、验证方式和隐私处理说明
- ✅ 支持在线体验（HTML/H5 互动产品）
- ✅ 在主流桌面浏览器环境下可正常运行
- ✅ 主题积极健康，适合校园传播
- ✅ 聚焦AI互动产品与心理成长领域

## 许可证

MIT License