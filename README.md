# WxDump Web

这是 [PyWxDump](https://github.com/xaoyaoo/PyWxDump) 的 Web 版，用于在浏览器中查看微信聊天记录。

## 功能特性

- 📱 微信聊天记录查看
- 📊 聊天数据统计分析
- 📈 可视化图表展示
- 💾 多种格式导出（HTML、JSON、CSV、PDF、DOCX等）
- 🔍 消息搜索和筛选
- 📷 图片、视频、音频消息支持

## 技术栈

- **前端框架**: Vue 3 + TypeScript
- **构建工具**: Vite
- **UI 组件**: Element Plus
- **图表库**: ECharts
- **HTTP 客户端**: Axios

## 快速开始

### 环境要求

- Node.js >= 16
- npm 或 yarn

### 安装

```bash
# 克隆项目
git clone https://github.com/nancy4567891011/wechat-chat-viewer.git

# 进入项目目录
cd wechat-chat-viewer

# 安装依赖
npm install
```

### 开发

```bash
# 启动开发服务器
npm run dev
```

### 构建

```bash
# 构建生产版本
npm run build
```

## 项目结构

```
wxdump_web/
├── public/                 # 静态资源
├── src/
│   ├── api/               # API 接口
│   ├── assets/            # 资源文件
│   ├── components/        # 组件
│   │   ├── chat/         # 聊天相关组件
│   │   ├── chatBackup/   # 导出功能组件
│   │   ├── stats/        # 统计分析组件
│   │   └── utils/        # 工具组件
│   ├── router/           # 路由配置
│   ├── utils/            # 工具函数
│   └── views/            # 页面视图
├── package.json
└── vite.config.ts
```

## 使用说明

1. 确保已安装并运行 [PyWxDump](https://github.com/xaoyaoo/PyWxDump) 后端服务
2. 启动本项目的开发服务器
3. 在浏览器中访问 `http://localhost:8080`
4. 开始查看和分析微信聊天记录

## 相关项目

- [PyWxDump](https://github.com/xaoyaoo/PyWxDump) - 微信数据库读取工具

## 许可证

本项目基于 MIT 许可证开源。

## 贡献

欢迎提交 Issue 和 Pull Request！

## 免责声明

本工具仅用于个人学习和研究目的，请遵守相关法律法规，不得用于非法用途。