ApexIDE 项目构想

## 🌍 多语言支持

应用支持以下语言：
- 🇨🇳 简体中文 (`values-zh-rCN/`)
- 🇹🇼 繁体中文 (`values-zh-rTW/`)
- 🇺🇸 英语 (`values/`)
- 🇯🇵 日语 (`values-ja/`)
- 🇰🇷 韩语 (`values-ko/`)
- 🇪🇸 西班牙语 (`values-es/`)

语言切换通过 `LanguageManager` 实现，支持运行时动态切换。

## 🎨 主题系统

应用支持三种主题模式：
- 🌞 亮色主题
- 🌙 暗色主题
- 🔄 跟随系统

主题配置通过 `ThemeManager` 管理，使用 Material Design 3 设计规范。

## 📱 主要功能

### 1. 文件管理器 (`FileManagerPage.kt`)
- 浏览和管理文件系统
- 支持创建文件/文件夹
- 支持重命名、删除操作
- 支持显示隐藏文件
- 支持图片和 APK 文件预览
- 支持多种文件类型图标和着色

### 2. 代码编辑器 (`EditorScreen.kt`)
- 基于 Sora 编辑器的代码编辑功能
- 支持语法高亮
- 支持多种编程语言（Java, Kotlin, Python, JavaScript 等）
- 文件保存和加载

### 3. Git 管理 (`GitManagerPage.kt`)
- Git 仓库管理
- 克隆 Git 仓库功能

### 4. AI 聊天 (`AIChatPage.kt`)
- AI 辅助编程功能

### 5. 搜索替换 (`SearchReplacePage.kt`)
- 文件内容搜索和替换

### 6. 插件系统 (`PluginManagerPage.kt`)
- 插件管理和扩展功能

## 🛠️ 技术栈

- **语言**: Kotlin + Java
- **UI 框架**: Jetpack Compose
- **架构**: MVVM
- **导航**: Navigation Compose
- **异步**: Kotlin Coroutines
- **状态管理**: StateFlow / LiveData
- **图片加载**: Coil
- **权限管理**: XXPermissions
- **代码编辑器**: Sora Editor
- **依赖注入**: ViewModel Compose

## 📝 开发规范

### 代码组织
- 按功能模块组织代码
- 使用包名清晰区分不同层级
- UI 组件使用 Composable 函数
- ViewModel 管理业务逻辑和状态

### 命名规范
- Kotlin 文件使用 PascalCase（如 `MainActivity.kt`）
- 函数和变量使用 camelCase
- 常量使用 UPPER_SNAKE_CASE
- Composable 函数使用 PascalCase

### 资源文件
- 字符串资源统一放在 `values/strings.xml`
- 多语言资源放在对应的 `values-*/strings.xml`
- 图标资源放在 `drawable/` 目录
- 使用有意义的资源名称

## 🧪 测试

- **单元测试**: `test/` 目录
- **集成测试**: `androidTest/` 目录

## 📦 依赖说明

主要依赖项（详见 `app/build.gradle.kts`）：
- Jetpack Compose BOM
- Material Design 3
- Navigation Compose
- Lifecycle & ViewModel
- Coil (图片加载)
- XXPermissions (权限管理)
- Sora Editor (代码编辑器)
- Kotlin Coroutines

## 🔧 构建要求

- **最小 SDK**: 28 (Android 9.0)
- **目标 SDK**: 35
- **编译 SDK**: 36
- **Kotlin 版本**: 2.0.21
- **Java 版本**: 17

## 📄 许可证

请查看项目根目录的 LICENSE 文件。

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

---

**注意**: 本目录是应用的核心源代码目录，修改代码时请遵循项目的架构模式和编码规范。

