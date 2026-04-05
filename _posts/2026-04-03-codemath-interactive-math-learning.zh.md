---
layout: post
title: "CodeMath：交互式数学学习平台"
date: 2026-04-03 00:00:00 +0800
tags: [数学, react, typescript, 教育, 开源, 可视化]
excerpt: "通过丰富的动画、3D 效果和交互式演示，让计算机科学数学变得生动有趣。"
lang: zh
slug: codemath-interactive-math-learning
permalink: /blog/zh/codemath-interactive-math-learning
---

![CodeMath 首页](/images/codemath-home.png)

# CodeMath：交互式数学学习平台 🧮

我很高兴介绍我的最新开源项目 — **CodeMath**，一个用现代 web 技术构建的交互式数学学习平台。

## 灵感来源

数学是计算机科学的基础，但传统的学习方法往往让它显得抽象和令人生畏。我想创造一些不同的东西 — 一个通过**交互**和**可视化**让数学概念活起来的平台。

CodeMath 的灵感来自 [结城浩](https://www.hyuki.com/) 的书籍《程序员的数学》。章节主题和学习路径遵循该书的结构，而所有代码实现、交互组件和可视化都是原创工作。

## 核心功能

### 🎮 交互式章节
每一章都包含动手交互内容，帮助你通过实践理解概念：

- **第 1 章：零的故事** — 进制转换器、位运算可视化
- **第 2 章：逻辑** — 逻辑门游乐场、真值表生成器
- **第 3 章：余数** — 日期计算器、国际象棋魔术
- **第 4 章：数学归纳法** — 多米诺骨牌模拟器
- **第 5 章：排列组合** — 卡片实验室、韦恩图
- **第 6 章：递归** — 汉诺塔、分形
- **第 7 章：指数级爆炸** — 折纸、二分 vs 线性搜索
- **第 8 章：不可解问题** — 停机问题模拟器
- **附录：机器学习** — 感知机训练场

### 🌏 智能本地化
- **双语支持**（中文/英文）
- 自动检测你的首选语言
- 轻松切换语言

### 🚀 开发者体验
- **一键启动** — `./start.sh` 处理一切
- **首次运行时自动安装依赖**
- **后台服务器模式**，带 PID 管理
- **完整日志记录**到 `logs/startup.log`
- **智能镜像源** — 在中国自动切换到淘宝 npm 源

## 技术栈

### 前端
- **React 19** — 最新特性和性能
- **TypeScript** — 类型安全开发
- **Vite** — 极速构建工具
- **Tailwind CSS** — 原子化 CSS
- **shadcn/ui** — 美观、可访问的组件

### 动画与可视化
- **GSAP** — 专业级动画
- **Three.js** — 3D 渲染和效果
- **KaTeX** — 快速、美观的数学排版
- **Lenis** — 平滑滚动体验

## 快速开始

### 克隆并运行

```bash
git clone https://github.com/hugcosmos/CodeMath.git
cd CodeMath
./start.sh
```

脚本会：
1. 询问你是否在中国大陆（自动配置 npm 镜像源）
2. 首次运行时自动安装依赖
3. 在后台启动开发服务器
4. 将所有输出记录到 `logs/startup.log`

访问：[http://localhost:5173/](http://localhost:5173/)

### 手动设置

```bash
cd app
npm install
npm run dev    # 启动开发服务器
npm run build  # 构建生产版本
npm run preview  # 预览生产构建
```

## 在线演示

**立即体验**：[https://codemath.pages.dev/](https://codemath.pages.dev/)

## 项目结构

```
CodeMath/
├── app/                    # 主应用
│   ├── src/
│   │   ├── components/     # 可复用组件
│   │   ├── sections/       # 页面区块
│   │   ├── chapters/       # 章节交互内容
│   │   ├── hooks/          # 自定义 hooks
│   │   ├── lib/            # 工具函数
│   │   └── i18n/           # 国际化配置
│   ├── package.json
│   └── vite.config.ts
├── logs/                   # 日志目录
├── start.sh                # 启动脚本 ⭐
├── stop.sh                 # 停止脚本 ⭐
├── README.md               # 项目说明
└── tech-spec.md            # 技术规范
```

## 常见问题

**Q: 如果端口 5173 被占用怎么办？**
A: 运行 `./stop.sh` 停止现有进程，或在 `app/vite.config.ts` 中手动更改端口。

**Q: 如何切换 npm 源？**
A: 脚本会自动检测环境。手动切换：
```bash
npm config set registry https://registry.npmmirror.com  # 淘宝
npm config set registry https://registry.npmjs.org       # 官方
```

**Q: 依赖安装失败？**
A: 删除 `app/node_modules` 和 `app/package-lock.json`，然后重新运行 `./start.sh`。

## 理念

> 💡 **数学不应该只是公式和定理 — 它应该是可触摸的、可探索的。**

CodeMath 体现了这一理念，让抽象概念变得可视化、可交互、有趣。

## 许可证

MIT License — 完全开源，欢迎贡献！

## 链接

- **GitHub**: [github.com/hugcosmos/CodeMath](https://github.com/hugcosmos/CodeMath)
- **在线演示**: [https://codemath.pages.dev/](https://codemath.pages.dev/)


Made with 💙 by Nicky & AI
