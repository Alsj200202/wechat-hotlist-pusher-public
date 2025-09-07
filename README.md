# WeChat Hotlist Pusher

微信热榜推送工具 - 自动获取并推送热门话题到微信

## 功能特性

- 🔥 自动获取各大平台热榜数据
- 📱 微信消息推送功能
- ⏰ 定时推送热榜内容
- 📊 热榜数据统计分析
- 🎯 智能筛选热门话题
- 📈 可视化数据展示

## 支持的热榜平台

- 微博热搜
- 知乎热榜
- 百度热搜
- 抖音热榜
- B站热门
- 头条热榜

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
git clone https://github.com/nancy4567891011/wechat-hotlist-pusher.git

# 进入项目目录
cd wechat-hotlist-pusher

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
wechat-hotlist-pusher/
├── public/                 # 静态资源
├── src/
│   ├── api/               # API 接口
│   ├── assets/            # 资源文件
│   ├── components/        # 组件
│   │   ├── hotlist/      # 热榜相关组件
│   │   ├── pusher/       # 推送功能组件
│   │   ├── stats/        # 统计分析组件
│   │   └── utils/        # 工具组件
│   ├── router/           # 路由配置
│   ├── utils/            # 工具函数
│   └── views/            # 页面视图
├── package.json
└── vite.config.ts
```

## 使用说明

1. 配置微信推送参数
2. 选择要监控的热榜平台
3. 设置推送时间和频率
4. 启动热榜监控服务
5. 自动推送热门内容到微信

## 配置说明

### 微信推送配置

```javascript
// 在 src/config/wechat.js 中配置
export const wechatConfig = {
  appId: 'your-app-id',
  appSecret: 'your-app-secret',
  templateId: 'your-template-id'
}
```

### 热榜平台配置

```javascript
// 在 src/config/platforms.js 中配置
export const platforms = {
  weibo: true,      // 微博热搜
  zhihu: true,      // 知乎热榜
  baidu: true,      // 百度热搜
  douyin: false,    // 抖音热榜
  bilibili: true,   // B站热门
  toutiao: false    // 头条热榜
}
```

## API 接口

### 获取热榜数据

```javascript
// GET /api/hotlist/:platform
// 获取指定平台的热榜数据

// GET /api/hotlist/all
// 获取所有平台的热榜数据
```

### 推送管理

```javascript
// POST /api/push/send
// 手动发送推送

// GET /api/push/history
// 获取推送历史
```

## 许可证

本项目基于 MIT 许可证开源。

## 贡献

欢迎提交 Issue 和 Pull Request！

## 免责声明

本工具仅用于个人学习和研究目的，请遵守相关法律法规和平台使用条款，不得用于商业用途或违法行为。