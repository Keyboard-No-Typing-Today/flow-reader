# Flow Reader

一个基于 Next.js 的 ePub 阅读器 Web 应用。

## 功能特性

- 网格布局
- 书内搜索
- 图片预览
- 自定义排版
- 高亮和注释
- 主题切换
- 数据导出
- 云存储支持

## 快速开始

### 环境要求

- Node.js >= 18.0.0
- pnpm 包管理器

### 安装依赖

```bash
pnpm install
```

### 构建生产版本

```bash
pnpm build
```

### 运行生产版本

```bash
pnpm start

```bash
pnpm dev
```

## Self-hosting

Before self-hosting, you should [setup the environment variables](#setup-the-environment-variables).

### Docker

You can use docker-compose:

```

应用将在 `http://localhost:3000` 上运行。

## 项目结构

```
flow/
├── apps/                # Reader 应用（Next.js）
│   ├── src/             # 源代码
│   ├── public/          # 静态资源
│   └── .next/           # 构建输出（生成后）
├── packages/
│   ├── epubjs/              # ePub 阅读器引擎
│   ├── internal/            # 内部共享工具
│   └── tailwind/            # Tailwind 配置
└── package.json             # 根配置
```

## 技术栈

- **Next.js 12** - React 框架
- **React 18** - UI 库
- **Epub.js** - ePub 渲染引擎
- **Tailwind CSS** - 样式框架
- **Dexie** - IndexedDB 封装
- **Recoil** - 状态管理
- **Turborepo** - Monorepo 工具

## 部署

构建完成后，可以通过以下方式部署：

1. **使用 Node.js 服务器**：运行 `pnpm start`

## License

参见 LICENSE 文件。
