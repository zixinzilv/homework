前端代码
# 📱 Uni-app 社交应用项目

一个基于 uni-app 3.0 + Vue 3 开发的跨平台社交应用，支持小程序、H5 等多端运行。

## ✨ 功能特性

### 🔐 用户系统
- **登录页面** - 支持手机号/密码登录，带有表单验证
- **注册页面** - 完整的注册流程，包含：
  - 用户名输入
  - 手机号验证（11位中国大陆手机号格式）
  - 密码强度校验（至少6位，仅支持大小写字母和数字）
  - 确认密码验证
  - 用户协议勾选

### 📝 内容功能
- **首页** - 内容流展示
- **详情页** - 帖子详情查看
  - 图片轮播展示
  - 点赞功能（带心跳动画效果）
  - 评论列表
  - 评论发布
- **发布页** - 内容发布功能

### 👤 个人中心
- **个人主页** - 用户信息展示
- **设置页面** - 应用设置
- **私信功能** - 消息通知

## 🛠️ 技术栈

- **框架**: uni-app 3.0.0
- **前端**: Vue 3.4.21
- **构建工具**: Vite 5.2.8
- **语言**: JavaScript
- **样式**: CSS (rpx 响应式单位)

## 📦 项目结构

```
├── pages/
│   ├── login/          # 登录页
│   ├── register/       # 注册页
│   ├── home/           # 首页
│   ├── detail/         # 详情页
│   ├── profile/        # 个人中心
│   ├── publish/        # 发布页
│   ├── message/        # 私信页
│   └── settings/       # 设置页
├── App.vue             # 应用入口
├── main.js             # 主入口文件
├── pages.json          # 页面配置
├── manifest.json       # 应用配置
└── package.json        # 依赖配置
```

## 🚀 快速开始

### 环境要求
- Node.js 14+
- HBuilderX (推荐) 或 VS Code + uni-app 插件

### 安装依赖
```bash
npm install
```

### 运行开发

#### H5端
```bash
npm run dev:h5
```

#### 微信小程序
```bash
npm run dev:mp-weixin
```

#### 其他平台
```bash
npm run dev:mp-alipay      # 支付宝小程序
npm run dev:mp-baidu       # 百度小程序
npm run dev:mp-qq          # QQ小程序
npm run dev:mp-toutiao     # 字节跳动小程序
```

### 构建打包

```bash
npm run build:h5           # H5打包
npm run build:mp-weixin    # 微信小程序打包
```

## 🎨 主要页面展示

### 登录 & 注册
- 渐变背景设计
- 实时表单验证
- 友好的错误提示

### 详情页
- 图片轮播
- 点赞动画效果（空心❤️ → 红心❤️）
- 评论交互

## ⚙️ 配置说明

### pages.json
- 配置了 8 个主要页面
- 底部 TabBar 包含首页和个人中心
- 全局导航栏设置为自定义样式

### manifest.json
需要补充的配置项：
- `name`: 应用名称
- `appid`: 应用ID（DCloud appid）
- `description`: 应用描述
- `mp-weixin.appid`: 微信小程序 AppID



