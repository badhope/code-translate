# 
# CIPHER NEXUS | 密码枢纽
![Version](https://img.shields.io/badge/version-2.0.0-neon-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-active-brightgreen)
> **探索古典与现代加密技术，在数字迷宫中寻找隐藏的真相。**
`CIPHER NEXUS` 是一个单文件网页应用，提供现代化的加密与解密服务。它不仅是工具，更是一个充满科技感与神秘氛围的密码世界入口。采用模块化架构设计，界面简洁，功能强大，支持大量文本处理。
---
## ✨ 核心特性
### 🏗️ 模块化架构
摒弃了传统工具的“堆砌式”布局，采用视图切换架构：
- **控制台**: 系统概览与快速入口
- **工作台**: 核心加解密操作区
- **档案库**: 历史记录管理与导出
- **密码图鉴**: 密码学知识百科
### 🔐 丰富的密码算法
支持 **16种** 主流密码算法，涵盖三大类别：
| 类别 | 算法 |
| :--- | :--- |
| **古典密码** | 摩斯密码、凯撒密码、埃特巴什、栅栏密码、维吉尼亚、培根密码、仿射密码、ROT13 |
| **现代编码** | Base64、URL编码、二进制、十六进制、ASCII码 |
| **哈希摘要** | MD5、SHA-1、SHA-256 (单向加密) |
### 🎨 沉浸式视觉体验
- **Glassmorphism (玻璃态)**: 半透明磨砂质感，层次分明。
- **Neon Cyberpunk (霓虹赛博)**: 深邃背景配合霓虹发光效果。
- **动态元素**: 浮动几何体、扫描线动画、网格背景。
- **专属图标**: 每种密码算法配备独特的 SVG 图标，告别枯燥。
### 🚀 强大的功能支持
- **海量文本**: 支持超长文本输入与处理，无字符限制。
- **文件交互**: 支持拖拽上传 `.txt` 文件，支持结果下载。
- **本地存储**: 操作历史自动保存到浏览器本地。
- **响应式设计**: 完美适配手机与电脑端。
---
## 🛠️ 技术栈
- **前端框架**: HTML5 + Native JavaScript (ES6+)
- **样式引擎**: Tailwind CSS (CDN)
- **加密库**: Crypto-JS (用于 SHA, MD5 等现代哈希算法)
- **图标库**: Font Awesome 6 + Custom SVG Icons
- **字体**: Orbitron (Display) + JetBrains Mono (Monospace)
---
## 📖 使用指南
### 1. 控制台
首页展示系统状态与四大功能模块入口。点击卡片即可进入对应功能。
### 2. 工作台
这是核心操作区域：
1.  **选择模式**: 点击顶部切换 `加密模式` 或 `解密模式`。
2.  **输入文本**: 在左侧输入框键入文本，或拖拽文件上传。
3.  **选择算法**: 在底部网格中选择一种密码算法（部分算法需配置参数）。
4.  **执行**: 点击 `执行加密/解密` 按钮，结果将显示在右侧。
### 3. 档案库
- 查看所有历史操作记录。
- 点击记录可快速恢复到工作台。
- 支持一键清空或导出为 JSON 文件。
### 4. 密码图鉴
浏览所有支持的密码算法简介、分类及特性，了解其背后的历史与原理。
---
## 🎨 设计理念
设计灵感来源于“数字迷宫”与“特工档案”。
- **配色**: 以深邃的 `Void Black` (#05080f) 为底，点缀 `Neon Blue` (#00f0ff) 和 `Neon Purple` (#bf00ff)，营造精密、悬疑的科技氛围。
- **交互**: 所有交互均带有微动效，按钮悬停时的光晕、卡片的浮起效果，旨在提供流畅的操作反馈。
- **极简主义**: 通过视图切换隐藏非必要元素，确保用户在任何时刻都专注于当前任务。
---
## 📦 部署与运行
本项目为单文件纯静态应用，无需后端服务器，无需安装依赖。
1.  下载 `index.html` 文件。
2.  双击文件直接在浏览器中打开即可使用。
或者部署在任何静态网站托管服务（如 GitHub Pages, Vercel, Netlify）上。
---
## 📜 更新日志
### v2.0.0 (Current)
- **重构**: 采用模块化视图架构，界面更简洁。
- **新增**: 增加 MD5, SHA-1, SHA-256, 培根密码, 仿射密码。
- **优化**: 全新 UI 设计，引入玻璃态与霓虹风格。
- **功能**: 支持文件拖拽上传、历史记录导出。
- **适配**: 完善移动端底部导航适配。
---
## 👨‍💻 作者
Designed & Developed by **GLM5**.
如果你喜欢这个项目，欢迎 Star ⭐ 支持！


# CIPHER NEXUS
## Version License Status

Explore classical and modern encryption technologies, seeking hidden truths within the digital maze. **CIPHER NEXUS** is a single-file web application providing modern encryption and decryption services. It's not just a tool, but a gateway to a cryptographic world filled with technological sophistication and mysterious atmosphere. Built with modular architecture design, featuring a clean interface, powerful functionality, and support for large-scale text processing.

---

## ✨ Core Features

### 🏗️ Modular Architecture
Abandoning the traditional "stacked" layout of conventional tools, adopting a view-switching architecture:

| Module | Description |
|--------|-------------|
| **Console** | System overview and quick access entry points |
| **Workbench** | Core encryption/decryption operation area |
| **Archive** | History record management and export |
| **Cipher Gallery** | Cryptography knowledge encyclopedia |

### 🔐 Rich Cryptographic Algorithms
Supports **16 mainstream cipher algorithms**, covering three major categories:

| Category | Algorithms |
|----------|------------|
| **Classical Ciphers** | Morse Code, Caesar Cipher, Atbash, Rail Fence, Vigenère, Bacon's Cipher, Affine Cipher, ROT13 |
| **Modern Encoding** | Base64, URL Encoding, Binary, Hexadecimal, ASCII Code |
| **Hash Digests** | MD5, SHA-1, SHA-256 (One-way Encryption) |

### 🎨 Immersive Visual Experience
- **Glassmorphism**: Translucent frosted texture with clear layering
- **Neon Cyberpunk**: Deep background with neon glowing effects
- **Dynamic Elements**: Floating geometries, scanline animations, grid backgrounds
- **Exclusive Icons**: Each cipher algorithm equipped with unique SVG icons, saying goodbye to boredom

### 🚀 Powerful Functionality Support
- **Massive Text**: Supports ultra-long text input and processing, no character limits
- **File Interaction**: Supports drag-and-drop upload of `.txt` files, supports result download
- **Local Storage**: Operation history automatically saved to browser local storage
- **Responsive Design**: Perfectly adapts to both mobile and desktop devices

---

## 🛠️ Technology Stack

| Component | Technology |
|-----------|------------|
| **Frontend Framework** | HTML5 + Native JavaScript (ES6+) |
| **Style Engine** | Tailwind CSS (CDN) |
| **Encryption Library** | Crypto-JS (for SHA, MD5, and other modern hash algorithms) |
| **Icon Library** | Font Awesome 6 + Custom SVG Icons |
| **Fonts** | Orbitron (Display) + JetBrains Mono (Monospace) |

---

## 📖 User Guide

### 1. Console
The homepage displays system status and entry points for the four major functional modules. Click on cards to access corresponding functions.

### 2. Workbench
This is the core operation area:

1. **Select Mode**: Click to switch between **Encrypt Mode** or **Decrypt Mode** at the top
2. **Input Text**: Type text in the left input box, or drag-and-drop to upload files
3. **Select Algorithm**: Choose a cipher algorithm from the bottom grid (some algorithms require parameter configuration)
4. **Execute**: Click the **Execute Encryption/Decryption** button, results will display on the right

### 3. Archive
- View all historical operation records
- Click on records to quickly restore to workbench
- Supports one-click clear or export as JSON file

### 4. Cipher Gallery
Browse introductions, classifications, and features of all supported cipher algorithms, understanding the history and principles behind them.

---

## 🎨 Design Philosophy

Design inspiration comes from **"Digital Maze"** and **"Agent Archives"**.

| Aspect | Description |
|--------|-------------|
| **Color Scheme** | Based on deep **Void Black** (#05080f), accented with **Neon Blue** (#00f0ff) and **Neon Purple** (#bf00ff), creating a precise and suspenseful technological atmosphere |
| **Interaction** | All interactions include micro-animations, button hover glows, card floating effects, aiming to provide smooth operation feedback |
| **Minimalism** | Hides non-essential elements through view switching, ensuring users focus on current tasks at any moment |

---

## 📦 Deployment & Running

This project is a **single-file pure static application**, requiring no backend server and no dependency installation.

1. Download the `index.html` file
2. Double-click the file to open directly in browser for use
3. Or deploy on any static website hosting service (such as **GitHub Pages**, **Vercel**, **Netlify**)

---

## 📜 Changelog

### v2.0.0 (Current)
| Type | Description |
|------|-------------|
| **Refactor** | Adopted modular view architecture, cleaner interface |
| **New** | Added MD5, SHA-1, SHA-256, Bacon's Cipher, Affine Cipher |
| **Optimize** | Brand new UI design, introducing glassmorphism and neon style |
| **Feature** | Supports file drag-and-drop upload, history record export |
| **Adaptation** | Improved mobile bottom navigation adaptation |

---

## 👨‍💻 Author

**Designed & Developed by GLM5**

If you like this project, welcome to **Star ⭐** to support!

---




