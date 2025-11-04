# toolkit_core

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE.txt)
[![Version](https://img.shields.io/badge/version-1.0.0-brightgreen.svg)](oh-package.json5)

## 简介

`toolkit_core` 是一个面向 OpenHarmony/HarmonyOS 应用开发的核心基础工具包，提供了一系列常用的工具函数和组件，帮助开发者更高效地构建 HarmonyOS 应用。

## 特性

- 🚀 轻量级设计，零依赖
- 📦 完整的 TypeScript 类型支持
- 🔧 开箱即用的工具函数
- 📱 专为 HarmonyOS/OpenHarmony 平台优化
- ✅ 完善的单元测试覆盖

## 安装

### 通过 ohpm 安装

```bash
ohpm install @jackson_chen/toolkit_core
```

### 通过源码安装

1. 克隆仓库

```bash
git clone https://github.com/chenjing1129/OpenHarmony-HAR.git
```

2. 在项目中引用本地模块

## 快速开始

### 导入模块

在你的项目中导入需要的组件：

```typescript
import { MainPage } from "@jackson_chen/toolkit_core";
```

### 使用示例

```typescript
// 在你的页面中使用 MainPage 组件
@Entry
@Component
struct Index {
  build() {
    Column() {
      MainPage()
    }
  }
}
```

## API 文档

### 组件

#### MainPage

一个基础的页面组件示例。

**属性：**

- `message`: string - 显示的消息文本

**示例：**

```typescript
MainPage();
```

## 项目结构

```
toolkit_core/
├── src/
│   ├── main/
│   │   ├── ets/
│   │   │   └── components/      # 组件目录
│   │   │       └── MainPage.ets
│   │   ├── module.json5         # 模块配置
│   │   └── resources/           # 资源文件
│   ├── ohosTest/                # 单元测试
│   └── test/                    # 本地测试
├── Index.ets                    # 导出入口
├── oh-package.json5             # 包配置文件
├── build-profile.json5          # 构建配置
├── LICENSE.txt                  # 开源协议
├── README.md                    # 项目说明
└── CHANGELOG.md                 # 版本日志
```

## 开发指南

### 环境要求

- DevEco Studio: 5.0.0 或更高版本
- SDK: HarmonyOS NEXT API 12 或更高版本
- Node.js: 18.x 或更高版本

### 本地开发

1. 克隆项目

```bash
git clone https://github.com/chenjing1129/OpenHarmony-HAR.git
cd toolkit/toolkit_core
```

2. 安装依赖

```bash
ohpm install
```

3. 运行测试

```bash
# 运行单元测试
ohpm test
```

4. 构建项目

```bash
# 构建 HAR 包
hvigorw assembleHar
```

### 发布 HAR 包

1. 更新版本号（在 `oh-package.json5` 中）
2. 更新 `CHANGELOG.md`
3. 构建发布版本

```bash
hvigorw assembleHar --mode release
```

4. 发布到 ohpm 仓库

```bash
ohpm publish
```

## 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建你的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的改动 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启一个 Pull Request

## 版本历史

详见 [CHANGELOG.md](CHANGELOG.md)

## 许可证

本项目采用 [Apache License 2.0](LICENSE.txt) 开源协议。

## 作者

**jackson_chen**

## 相关链接

- [GitHub 仓库](https://github.com/chenjing1129/OpenHarmony-HAR.git)
- [HarmonyOS 官方文档](https://developer.harmonyos.com/)
- [OpenHarmony 官网](https://www.openharmony.cn/)

## 支持

如有问题或建议，请通过以下方式联系：

- 提交 [Issue](https://github.com/chenjing1129/OpenHarmony-HAR/issues)
- 发送邮件至作者

## 致谢

感谢所有为本项目做出贡献的开发者！

---

**注意**: 本项目仍在积极开发中，API 可能会有变动。建议在生产环境中使用稳定版本。
