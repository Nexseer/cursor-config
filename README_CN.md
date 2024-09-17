# cursor-config

👉 English | [简体中文](README_CN.md)

- [一、简介 💬](#一简介-)
- [二、核心优势 🌟](#二核心优势-)
- [三、订阅价格 💰](#三订阅价格-)
  - [Hobby 免费计划](#hobby-免费计划)
  - [Pro 每月 $20](#pro-每月-20)
  - [Business 每月 $40](#business-每月-40)
- [四、配置 🛠️](#四配置-️)
  - [1. 技巧 ⚙️](#1-技巧-️)
  - [2. 自定义配置 ⛏️](#2-自定义配置-️)
    - [外观配置](#外观配置)
    - [基础设置](#基础设置)
    - [Vim Mode 设置](#vim-mode-设置)
  - [3. 自定义按键 ⌨️](#3-自定义按键-️)
  - [4. 快捷键整理 📚](#4-快捷键整理-)
- [五、AI 功能 💥](#五ai-功能-)
  - [1. Cursor Tab ✍️](#1-cursor-tab-️)
  - [2. Cursor Chat 💬](#2-cursor-chat-)
  - [3. Ctrl K ⛏️](#3-ctrl-k-️)
  - [4. Prompt 提示词 📖](#4-prompt-提示词-)
  - [5. 自定义规则 📐](#5-自定义规则-)
  - [6. Composer 💻](#6-composer-)
- [六、插件](#六插件)
  - [Auto Close Tag](#auto-close-tag)
  - [Auto Import](#auto-import)
  - [Auto Rename Tag](#auto-rename-tag)
  - [C/C++](#cc)
  - [Cairo 1.0](#cairo-10)
  - [Clang-Format](#clang-format)
  - [Code Runner](#code-runner)
  - [Database Client JDBC](#database-client-jdbc)
  - [DotENV](#dotenv)
  - [ES7 React/Redux/GraphQL/React-Native snippets](#es7-reactreduxgraphqlreact-native-snippets)
  - [ESLint](#eslint)
  - [Even Better TOML](#even-better-toml)
  - [GitLens — Git supercharged](#gitlens--git-supercharged)
  - [Image Preview](#image-preview)
  - [Live Server](#live-server)
  - [Markdown Preview Enhanced](#markdown-preview-enhanced)
  - [Mojo 🔥](#mojo-)
  - [MySQL](#mysql)
  - [Npm Intellisense](#npm-intellisense)
  - [Path Intellisense](#path-intellisense)
  - [Pine Script Syntax Highlighter](#pine-script-syntax-highlighter)
  - [Prettier - Code formatter](#prettier---code-formatter)
  - [Pylance](#pylance)
  - [Python](#python)
  - [Regex Previewer](#regex-previewer)
  - [rust-analyzer](#rust-analyzer)
  - [Snazzy Operator](#snazzy-operator)
  - [Solidity](#solidity)
  - [Tailwind CSS IntelliSense](#tailwind-css-intellisense)
  - [TODO Highlight](#todo-highlight)
  - [Trailing Spaces](#trailing-spaces)
  - [Vim](#vim)
  - [vscode-icons (Mac 版)](#vscode-icons-mac-版)
  - [YAML](#yaml)
  - [Zig Language](#zig-language)

👉 [Cursor 官网](https://www.trycursor.com/)

👉 [Cursor 论坛](https://forum.cursor.com/)

👉 [Cursor 文档](https://docs.cursor.com/get-started/migrate-from-vscode)

> 代码编辑器（Code Editor）通常是轻量级的，主要聚焦于编辑源代码，提供基础的代码编辑功能，如语法高亮、文本编辑、文件管理等。代码编辑器通常具有高度的可定制性和扩展性，允许用户通过安装插件来增加额外的功能，如语法检查、版本控制等。代码编辑器通常不绑定特定的开发框架或语言，其相较于 IDE（Integrated Development Environment，集成开发环境）由于功能较少，通常更快，启动迅速，占用系统资源较少。

# 一、简介 💬

> Built to make you extraordinarily productive, Cursor is the best way to code with AI.

Cursor 编辑器定位是智能 AI 代码编辑器，旨在通过人工智能技术帮助开发者更高效地编写和编辑代码。Cursor 编辑器在**继承 VS Code 强大功能的基础**上（VS Code 到 Cursor 的迁移成本几乎是 0），进一步整合了先进的 AI 技术，极大地提升了编程的便捷性和效率。

> 迁移 VS Code 配置：导航到 Cursor 设置（`ctrl shift j`） > 通用 > 帐户

![image](https://github.com/user-attachments/assets/f10ffb9a-3e6a-4772-95fe-91832250bc9d)

对比 Github Copilot，Cursor 的最大亮点在于其强大的索引功能。它能够**基于整个项目构建索引**，这意味着 Cursor 不仅仅是简单地提供代码片段的补全，而是能够深入理解整个项目的结构和逻辑。这种全局的理解能力使得 Cursor 能够提供更加精准、更加符合项目整体需求的代码建议和补全。

在代码重构方面，Cursor 表现出色。它不仅能够轻松处理基础的重构任务，如变量重命名、文件移动和引用自动修改，还能借助 AI 的力量进行更复杂的重构操作。例如，它可以智能地建议函数移动、参数重构，甚至是代码抽取和优化。Cursor 的 AI 功能还可以理解开发者的意图，提供上下文相关的建议和改进，这使得高级重构变得更加直观和高效。

# 二、核心优势 🌟

👉 [Features | Cursor - The AI-first Code Editor](https://www.cursor.com/features#codebase-wide)

1. **了解您的代码库** —— `Chat`：
   用户可以通过聊天界面直接查询代码库中的信息或引用特定的文件或文档。这种方式非常适合快速获取方案或进行代码审查，用户还可以通过简单的点击即可使用模型生成的代码片段。

2. **Copilot++** —— `Tab`：
   通过 Cursor 的 Copilot++ 功能，只需按下 Tab 键，编辑器就能预测并自动完成代码，根据上下文推荐下一步可能的代码编辑。这不仅加快了代码编写速度，还提高了开发效率，尤其是在处理复杂代码时能够提供实时的智能支持。

3. **使用自然语言编辑** —— `Ctrl K`：
   Cursor 的 `Ctrl K` 功能允许用户使用自然语言指令来编写和更新代码。这意味着用户可以通过简单的文本提示，如“增加一个新方法”或“更新这个函数的参数”，快速执行复杂的编程任务。

4. **完整而强大的生态系统**：
   依靠 VS Code ，拥有数以千计的扩展插件，涵盖了各种编程语言、框架、工具和功能，用户可以轻松找到并安装满足特定需求的扩展。

# 三、订阅价格 💰

👉 [Pricing | Cursor](https://www.trycursor.com/pricing)

🎉 两周 Pro 试用期！！

## Hobby 免费计划

每月（一共） 2000 个代码补全（completions）

50 个慢速优先的高级请求（slow premium requests）

100 次 Cursor-small 模型的使用（Cursor-small 是一个更快的模型，适用于快速编辑任务）

## Pro 每月 $20

包括所有 Hobby 计划内容

提供无限制的代码补全

每月 500 个快速优先的高级请求（高级模型包括 GPT-4、GPT-4o 和 Claude 3.5 Sonnet）

无限制的慢速高级请求

无限制的 Cursor-small 使用

每天 10 次 Claude Opus 使用。

## Business 每月 $40

包括 Pro 计划内容，并增加了集中式账单、管理员使用情况仪表板、强制隐私模式和 OpenAI/Anthropic 零数据保留政策。隐私模式确保代码仅存储在用户的设备上，不会用于训练。Cursor 的某些功能不支持通过 API 密钥计费。如果用户超出计划限制，Cursor 会请求用户升级计划。

# 四、配置 🛠️

## 1. 技巧 ⚙️

- 不开启自动保存：自动保存可以避免因忘记保存而导致的数据丢失，但是频繁的自动保存操作可能会增加系统的 I/O 负担，尤其是在处理大型项目或复杂文件时，可能会导致编辑器的响应速度变慢。

- 自动生成 Git Commit Message：`ctrl l` 进入 AI Chat 面板，输入`@Commit (Diff of Working State)`获取更改，再输入对应的 prompt `give me a one-line commit message`。

- Codebase 索引忽略：快捷键 `ctrl shift j`  打开 Cursor Settings 面板，进行如下操作，或者项目添加`.cursorignore`，添加的这些文件和目录将不会被 Cursor 编辑器索引，从而提高编辑器的性能和搜索效率。

![image](https://github.com/user-attachments/assets/ee4a1a68-7ce6-439f-a395-2640c0fe8bf9)

## 2. 自定义配置 ⛏️

打开设置，有以下两种办法：

1. 快捷键  `ctrl ,`

2. 打开命令面板  `crtl shift p`，输入  `Open VS Code Settings`

> 设置面板提供了一个用户友好的图形界面，用户可以通过点击和选择来修改配置，而不需要直接编辑 JSON 文件。

`settings.json` 文件提供了更高的灵活性和精细控制，我们选择 `settings.json`。

![image](https://github.com/user-attachments/assets/15389db1-d017-42fd-b767-b8e0d98e5cbc)

### 外观配置

```json
// 窗口缩放级别设置为 1，表示界面放大到 110%
"window.zoomLevel": 1,
// 垂直显示
"workbench.activityBar.orientation": "vertical",
// 主题配置
"workbench.colorTheme": "Snazzy Operator",
// 图标主题设置
"workbench.iconTheme": "vscode-icons-mac",
// 启用平滑滚动
"workbench.list.smoothScrolling": true,
// 聊天编辑器的字体大小设置
"chat.editor.fontSize": 18,
// 文件夹不使用紧凑模式显示
"explorer.compactFolders": false,
// 编辑器的字体大小设置
"editor.fontSize": 24,
// 编辑器的字体设置
"editor.fontFamily": "Cascadia Code NF",
// 编辑器的字体设置
"editor.inlayHints.fontFamily": "Consolas",
"editor.minimap.enabled": true,
// 保存时自动格式化代码
"editor.formatOnSave": true,
// 相对行号模式
"editor.lineNumbers": "relative",
// 光标上下方始终可见的行数
"editor.cursorSurroundingLines": 6,
// 启用光标的平滑动画
"editor.cursorSmoothCaretAnimation": "on",
// 启用括号对的活动引导线
"editor.guides.bracketPairs": "active",
// 自动插入闭合的括号
"editor.autoClosingBrackets": "always",
// 启用悬停提示的粘滞效果
"editor.hover.sticky": true,
// 启用粘滞滚动功能
"editor.stickyScroll.enabled": true,
// 终端的字体大小设置
"terminal.integrated.fontSize": 16,
// 终端的字体设置
"terminal.integrated.fontFamily": "Cascadia Code NF"
```

### 基础设置

```json
// 重新打开时，不会恢复任何之前打开的窗口
"window.restoreWindows": "none",
// 禁用通过鼠标滚轮缩放编辑器字体大小的功能
"editor.mouseWheelZoom": false,
// 保存时自动执行 ESLint 的 `fixAll` 操作，修复所有可以自动修复的问题
"editor.codeActionsOnSave": {
  "source.fixAll.eslint": "explicit"
},
// mdx 文件关联为 markdown 文件类型
"files.associations": {
  "*.mdx": "markdown"
},
// 保存文件时自动删除行尾的空白字符
"files.trimTrailingWhitespace": true,
// 不显示推荐的扩展
"extensions.ignoreRecommendations": true,
// 设置 Prettier 作为默认的代码格式化工具
"editor.defaultFormatter": "esbenp.prettier-vscode",
// 配置 Prettier 使用单引号而不是双引号
"prettier.singleQuote": true,
// 特定语言的格式化工具设置
"[cpp]": {
  "editor.defaultFormatter": "xaver.clang-format"
},
"[c]": {
  "editor.defaultFormatter": "xaver.clang-format"
},
"[html]": {
  "editor.defaultFormatter": "vscode.html-language-features"
},
"[css]": {
  "editor.defaultFormatter": "vscode.css-language-features"
},
"[scss]": {
  "editor.defaultFormatter": "vscode.css-language-features"
},
"[python]": {
  "editor.defaultFormatter": "ms-python.python"
},
"[toml]": {
  "editor.defaultFormatter": "tamasfe.even-better-toml"
},
"[rust]": {
  "editor.defaultFormatter": "rust-lang.rust-analyzer"
},
// 搜索时排除的文件和文件夹
"search.exclude": {
  "**/*.snap": true,
  "**/.git": true,
  "**/.github": false,
  "**/.nuxt": true,
  "**/.output": true,
  "**/.pnpm": true,
  "**/.vscode": true,
  "**/.yarn": true,
  "**/node_modules": true,
  "**/out/**": true,
  "**/package-lock.json": true,
  "**/pnpm-lock.yaml": true,
  "**/temp": true,
  "**/yarn.lock": true,
  "**/CHANGELOG*": true,
  "**/LICENSE*": true
},
// 文件扫描时要排除的文件和目录模式
"file_scan_exclusions": [
  "**/.git",
  "**/.svn",
  "**/.hg",
  "**/CVS",
  "**/.DS_Store",
  "**/Thumbs.db",
  "**/.classpath",
  "**/.settings",
  "**/vendor",
  "**/.tmp*"
],
```

### Vim Mode 设置

vsocde-vim 中内置了很多插件，使用它们可以快速的进行某一些操作。

- Easymotion 插件，通过以下的按键组合，你可以快速的定位到任何你想修改的行中：`<leader><leader>s<char>`，允许用户通过简单的键盘操作快速跳转到光标附近的任意位置，提高导航效率。

- 内置的 `vim-commentary` 插件，可视模式下的 `gc` 和普通模式下的 `gcc` 起切换注释作用。

- vim-surround 插件，如果你想修改、或者删除单引号和双引号：

```
ds<existing>
cs<existing><desired>

# 删除以下的[]
[1, 2, 3] -> ds[

# 将以下的[]修改为()
[1, 2, 3] -> cs[(
```

```json
// 设置 Vim 的 leader 键为空格键
"vim.leader": "<space>",
// 启用 EasyMotion 插件功能
"vim.easymotion": true,
// 允许 Vim 使用系统剪贴板
"vim.useSystemClipboard": true,
// 普通模式下的非递归键绑定
"vim.normalModeKeyBindingsNonRecursive": [
  {
    "before": ["H"],
    "commands": ["workbench.action.previousEditorInGroup"]
  },
  {
    "before": ["L"],
    "commands": ["workbench.action.nextEditorInGroup"]
  },
  {
    "before": ["K"],
    "commands": ["editor.action.showHover"]
  },
  {
    "before": ["g", "h"],
    "commands": ["cursorHome"]
  },
  {
    "before": ["g", "l"],
    "commands": ["cursorEnd"]
  },
  {
    "before": ["g", "d"],
    "commands": ["editor.action.revealDefinition"]
  },
  {
    "before": ["g", "D"],
    "commands": ["editor.action.revealDeclaration"]
  },
  {
    "before": ["g", "r"],
    "commands": ["editor.action.goToReferences"]
  },
  {
    "before": ["g", "i"],
    "commands": ["editor.action.goToImplementation"]
  },
  {
    "before": ["g", "b"],
    "commands": ["workbench.action.navigateBack"]
  },
  {
    "before": ["<leader>", "c", "f"],
    "commands": ["editor.action.formatDocument"]
  },
  {
    "before": ["<leader>", "c", "r"],
    "commands": ["editor.action.rename"]
  },
  {
    "before": ["<leader>", "e"],
    "commands": ["workbench.view.explorer"]
  },
  {
    "before": ["<leader>", "f", "f"],
    "commands": ["workbench.action.files.openFileFolder"]
  },
  {
    "before": ["<leader>", "f", "o"],
    "commands": ["workbench.action.gotoSymbol"]
  },
  {
    "before": ["<leader>", "f", "p"],
    "commands": ["workbench.action.openRecent"]
  },
  {
    "before": ["<leader>", "f", "q"],
    "commands": ["workbench.action.quickOpen"]
  },
  {
    "before": ["<leader>", "g", "["],
    "commands": ["gitlens.diffWithPrevious"]
  },
  {
    "before": ["<leader>", "g", "]"],
    "commands": ["gitlens.diffWithNext"]
  },
  {
    "before": ["<leader>", "g", "b"],
    "commands": ["gitlens.toggleFileBlame"]
  },
  {
    "before": ["<leader>", "g", "d"],
    "commands": ["gitlens.toggleFileChanges"]
  },
  {
    "before": ["<leader>", "g", "r"],
    "commands": ["git.revertSelectedRanges"]
  },
  {
    "before": ["<leader>", "m", "o"],
    "commands": ["markdown-preview-enhanced.openPreview"]
  },
  {
    "before": ["<leader>", "m", "p"],
    "commands": ["markdown-preview-enhanced.openPreviewToTheSide"]
  },
  {
    "before": ["<leader>", "p", "d"],
    "commands": ["workbench.actions.view.problems"]
  },
  {
    "before": ["<leader>", "p", "o"],
    "commands": ["workbench.action.output.toggleOutput"]
  },
  {
    "before": ["<leader>", "w", "c"],
    "commands": ["workbench.action.closeAllEditors"]
  },
  {
    "before": ["<leader>", "w", "h"],
    "commands": ["workbench.action.splitEditorRight"]
  },
  {
    "before": ["<leader>", "w", "v"],
    "commands": ["workbench.action.splitEditorDown"]
  },
  {
    "before": ["<C-a>"],
    "after": ["g", "g", "V", "G"]
  }
],
// 插入模式下的键绑定
"vim.insertModeKeyBindings": [],
// 命令行模式下的非递归键绑定
"vim.commandLineModeKeyBindingsNonRecursive": [],
"vim.handleKeys": {
  "<C-a>": false
}
```

> 📕 非递归键绑定：确保按下某个键组合时，只会执行与之直接关联的命令，而不会触发其他键绑定。

## 3. 自定义按键 ⌨️

打开按键设置，有以下两种办法：

1. 快捷键  `crtl shift k`

2. 打开命令面板  `crtl shift p`，输入  `Preferences:Open Keyboard Shortcuts`

3. 打开命令面板  `crtl shift p`，输入`Preferences:Open Default Keyboard Shortcuts (JSON)`

> 快捷键面板提供了一个用户友好的图形界面，用户可以通过点击和选择来修改配置，而不需要直接编辑 JSON 文件，并且可以查看可以配置的功能按键，复制 CommandID 即可。

`keybindings.json` 文件提供了更高的灵活性和精细控制，我们选择 `keybindings.json`。

![image](https://github.com/user-attachments/assets/6e1eea3e-66e5-4bd4-8c09-e43924b6256a)

```json
// Place your key bindings in this file to override the defaults

[
  {
    "key": "ctrl+shift+k",
    "command": "workbench.action.openGlobalKeybindings"
  },
  {
    "key": "ctrl+w",
    "command": "workbench.action.closeActiveEditor"
  },
  {
    "key": "ctrl+t",
    "command": "workbench.action.terminal.toggleTerminal",
    "when": "terminal.active"
  },

  {
    "key": "ctrl+w",
    "command": "workbench.action.closePanel",
    "when": "panelFocus"
  },

  {
    "key": "r",
    "command": "renameFile",
    "when": " explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus "
  },
  {
    "key": "d",
    "command": "deleteFile",
    "when": " explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus "
  },
  {
    "key": "x",
    "command": "filesExplorer.cut",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus"
  },
  {
    "key": "y",
    "command": "filesExplorer.copy",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !inputFocus"
  },
  {
    "key": "p",
    "command": "filesExplorer.paste",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceReadonly && !inputFocus"
  }
]
```

## 4. 快捷键整理 📚

**搜索**

| 快捷键         | 功能               |
| -------------- | ------------------ |
| `ctrl shift f` | 万能搜索           |
| `/` 或 `?`     | 搜索               |
| `n`            | （搜索）下一个结果 |
| `N`            | （搜索）上一个结果 |

**跳转操作**

| 快捷键 | 功能                   |
| ------ | ---------------------- |
| `g d`  | 跳转到定义             |
| `g D`  | 跳转到声明             |
| `g r`  | 跳转到引用             |
| `g i`  | 跳转到实现             |
| `g b`  | 返回到上一个光标位置   |
| `g h`  | 光标移动到当前行的行首 |
| `g l`  | 光标移动到当前行的行尾 |

**文件操作、explorer 面板**

| 快捷键       | 功能           |
| ------------ | -------------- |
| `<leader> e` | 文件资源管理器 |
| `c`          | 复制           |
| `d`          | 删除           |
| `p`          | 粘贴           |
| `r`          | 重命名         |
| `x`          | 剪切           |

**面板操作**

| 快捷键        | 功能                     |
| ------------- | ------------------------ |
| `ctrl t`      | 切换终端                 |
| `<space> p d` | 显示问题（如错误和警告） |
| `<space> p o` | 显示输出                 |
| `ctrl  w`     | 关闭面板                 |

**窗口操作**

| 快捷键        | 功能           |
| ------------- | -------------- |
| `<space> w c` | 关闭所有标签页 |
| `<space> w k` | 向上分割面板   |
| `<space> w j` | 向下分割面板   |
| `<space> w h` | 向左分割面板   |
| `<space> w l` | 向右分割面板   |

**基础操作**

| 快捷键         | 功能                 |
| -------------- | -------------------- |
| `ctrl alt n`   | 运行（Code Runner）  |
| `H`            | 上一个标签页         |
| `L`            | 下一个标签页         |
| `K`            | 显示悬停信息         |
| `<space> c f`  | 格式化               |
| `<space> c r`  | 重命名               |
| `<leader> f f` | 打开文件或文件夹     |
| `<space> f o`  | 查找文件大纲         |
| `<space> f p`  | 打开最近的项目       |
| `<space> f q`  | 快速打开项目下的文件 |
| `ctrl shift p` | 命令面板             |
| `ctrl shift d` | Run and Debug        |
| `ctrl shift k` | 快捷键设置           |
| `ctrl shift x` | 扩展插件             |
| `F11`          | 切换全屏模式         |

**Git 相关**

| 快捷键        | 功能                         |
| ------------- | ---------------------------- |
| `<space> g [` | 跳转到上一个 Git 更改        |
| `<space> g ]` | 跳转到下一个 Git 更改        |
| `<space> g b` | 切换`git blame`              |
| `<space> g d` | 切换显示当前  `hunk`  的差异 |
| `<space> g r` | 还原选定的  `hunks`          |

**Markdown 处理**

| 快捷键        | 功能                     |
| ------------- | ------------------------ |
| `<space> m o` | 打开 Markdown 预览       |
| `<space> m p` | 在侧边打开 Markdown 预览 |

**编辑操作**

| 快捷键     | 功能         |
| ---------- | ------------ |
| `ctrl a`   | 全选         |
| `ctrl w`   | 关闭标签页   |
| `ctrl y`   | 取消撤回操作 |
| `alt up`   | 向上移动行   |
| `alt down` | 向下移动行   |

# 五、AI 功能 💥

## 1. Cursor Tab ✍️

Cursor 的核心功能。不再局限于“补全”，而是**更广义的“编辑”**。

1. 自动完成代码
   在光标位置按下 `Tab` 键，Cursor Tab 会根据上下文提供建议。按下 `Tab` 键接受建议，Cursor Tab 可能会自动补全

2. 多行编辑
   可以一次修改多行，不再需要反复触发补全。

3. 修复 Linter 错误
   基于您最近的更改和 linter 错误提供建议。

4. 预测下一次改动
   自动跳转，比如我给一个函数加了类型注解，模型很快能 get 到我要给这个文件里的各种函数都加上类型注解，按 tab 就能跳到下一个改动自动 apply。

5. AI 支持下的重构
   自动帮忙生成编辑改动。

**使用方法：**

- 接受建议：按 `Tab` 键

- 拒绝建议：按 `Esc` 键或继续输入

- 逐字接受建议：按 `Ctrl/⌘ →`

## 2. Cursor Chat 💬

Cursor Chat 是一个基于 LLM 技术的聊天界面，允许用户通过对话的方式与 AI 进行互动。它不仅可以回答编程相关的问题，还能提供代码生成、错误修复、代码优化等多种功能，它自动包含整个代码库的上下文。可以用`@`操作符灵活指定 context，👉 详情查看[Cursor @ Symbols](https://docs.cursor.com/context/@-symbols/basic)

**使用方法：**

- 打开 AI 面板：按 `Ctrl/⌘ L`

- 输入问题或请求：在输入框中输入后按 `Enter`

## 3. Ctrl K ⛏️

`Ctrl K` 是 Cursor 编辑器中用于调用 AI 助手进行代码生成和编辑的快捷键。它能够根据用户的需求，自动生成代码、补全代码、修复代码错误、优化代码等，极大地提高了开发效率。（终端同样适用，达到类似 Wrap AI 的功能）

1. 代码生成
2. Bug 检测与修复
3. 代码解释
4. 文档生成
5. 代码优化建议
   ……

**使用方法：**

- 按 `Ctrl/⌘ K` 打开提示栏

- 使用 @ 符号引用其他上下文

- 输入指令并按 `Enter`

也可以选中一段代码，按下快捷键 `Ctrl/⌘ K`，直接输入需求或者问题，让 AI 帮你解决，绿色代码块是 AI 的生成结果，红色代码块是将被替换的原代码。

## 4. Prompt 提示词 📖

[Cursor Directory](https://cursor.directory/) 是一个专为 Cursor 编辑器设计的开源资源库，提供和收集了 Cursor 的各种配置文件和一系列提示词。这些提示词可以帮助 Cursor 编辑器更好地理解开发者的意图，从而提供更准确的代码补全、错误修复和其他智能化的编辑功能。

## 5. 自定义规则 📐

为 Cursor 添加自定义规则，如**全局规则**、**项目的特定规则**，这些将应用于 `Cursor Chat` 和 `Ctrl/⌘ K` 等功能。

**使用方法：**

- 全局规则：在 Cursor 设置 > 通用 > AI 规则

![image](https://github.com/user-attachments/assets/69168aa6-9522-44c4-a70b-a0d5c85cb8fe)

- 项目特定规则：在项目根目录创建 `.cursorrules` 文件，并添加相应规则。

## 6. Composer 💻

Composer 是一个多文件编辑工具，能够处理复杂的编程任务。它不仅限于单行或单文件的代码生成，还可以跨多个文件进行编辑和创建。

Composer 可以帮助开发者更快地完成复杂的编程任务，无论是生成新代码、优化现有代码，还是创建完整的应用程序，Composer 都能提供强大的支持。

**使用方法：**

- 确保功能已启用

![image](https://github.com/user-attachments/assets/7e4dfa33-197b-4d6c-b7d1-3ea32e0739a2)

- 按 `Ctrl/⌘ Shift I` 打开

# 六、插件

## Auto Close Tag

![image](https://github.com/user-attachments/assets/c9e8c7de-e23f-4fe0-bcf5-6a162ebe76f5)

用于自动补全 HTML、XML 和 JSX 标签的闭合标签，减少手动输入的工作量。

## Auto Import

![image](https://github.com/user-attachments/assets/ca730c98-f917-42cf-98c5-0a23160d2c51)

用于自动导入模块或库，减少手动输入导入语句的工作量。

## Auto Rename Tag

![image](https://github.com/user-attachments/assets/23d078de-ce9b-49cb-b979-fc5447ee75b4)

用于同步修改 HTML/XML 标签的起始标签和结束标签，确保标签名称一致。

## C/C++

![image](https://github.com/user-attachments/assets/dc1426ec-1a17-4283-a8de-af08c4820a12)

为 VS Code 提供跨平台的 C 和 C++ 开发支持，包括代码补全（IntelliSense）、调试和代码浏览功能。

## Cairo 1.0

![image](https://github.com/user-attachments/assets/82b43fc9-5758-4b50-a01a-7f606b3381c0)

为 Cairo 编程语言提供支持。

## Clang-Format

![image](https://github.com/user-attachments/assets/4ee48d97-8da5-49f8-b810-88d9f876e242)

够显著提升代码的整洁度和一致性，从而提高开发效率和代码质量。

## Code Runner

![image](https://github.com/user-attachments/assets/ab0ce013-52ac-4b3c-9376-02420302f530)

支持运行多种编程语言的代码片段或代码文件。

## Database Client JDBC

![image](https://github.com/user-attachments/assets/3b5293c3-a934-4ad0-94e4-ff381eec4adf)

用于在 VS Code 中管理和连接各种数据库，包括 MySQL、PostgreSQL、SQLite、Redis、ClickHouse 等，支持通过 JDBC 连接数据库。

## DotENV

![image](https://github.com/user-attachments/assets/6db4dc44-fd12-4395-b25a-bf6a6ea09b13)

用于在 VS Code 中处理 `.env` 文件，提供语法高亮、自动补全等功能。

## ES7 React/Redux/GraphQL/React-Native snippets

![image](https://github.com/user-attachments/assets/e3a0292c-e68a-48bb-8af6-b710f71897ff)

提供了一组代码片段，帮助快速编写 React、Redux、GraphQL 和 React-Native 代码。

## ESLint

![image](https://github.com/user-attachments/assets/6b1a272f-7194-4f2a-896a-26c9c0f1fc85)

帮助开发者在编写 JavaScript 和 TypeScript 代码时遵循一致的代码风格，并自动检测和修复代码中的问题。

## Even Better TOML

![image](https://github.com/user-attachments/assets/88022129-8b6b-4600-b60e-68752364a2ef)

提供 TOML 文件的语法高亮和验证功能。

## filesize

![image](https://github.com/user-attachments/assets/5664864d-3f4b-46a6-92e5-a31b91ed8fe0)

状态栏中显示当前文件的大小信息。点击状态栏中的文件大小信息，还可以查看文件的详细信息（如创建时间、修改时间等）。这对于管理项目中的文件和优化文件大小非常有用。

## GitLens — Git supercharged

![image](https://github.com/user-attachments/assets/3e0eae7a-965a-4710-9d0b-7b89234e7798)

旨在增强 Git 的功能，使开发者能够更方便地进行版本控制。

## Image Preview

![image](https://github.com/user-attachments/assets/740f473c-8b22-4bce-adef-520b348fdccd)

支持在编辑器中直接查看图像。

## Live Server

![image](https://github.com/user-attachments/assets/c78b62f1-9f5f-4c1d-9db1-d4a7c5c0ac56)

启动一个本地开发服务器，并在你保存文件时自动刷新浏览器，从而大大提高开发效率。

## Markdown Preview Enhanced

![image](https://github.com/user-attachments/assets/b1531b6e-4219-4bc3-af17-1ef3e3a9b652)

能够显著提升 Markdown 文件的编辑和预览体验，同时导出为 PDF。

## Mojo 🔥

![image](https://github.com/user-attachments/assets/60471bde-0c41-4060-b3a4-41d42cbc62b7)

提供 Mojo 编程语言的支持，包括语法高亮、代码补全等功能。

## MySQL

![image](https://github.com/user-attachments/assets/44437977-737e-4d7e-81fc-4254a23892b7)

管理和连接 MySQL 数据库，提供数据库浏览、查询执行等功能。

## Npm Intellisense

![image](https://github.com/user-attachments/assets/6cdef421-767a-4e0c-af3d-fee315ddf8a2)

通过自动补全 npm 模块的导入语句，简化了开发过程中的模块引入操作。

## Path Intellisense

![image](https://github.com/user-attachments/assets/51c4bf3f-5c65-4e21-8c96-237f74c97ece)

提供文件路径的自动补全功能，支持多种编程语言。

## Pine Script Syntax Highlighter

![image](https://github.com/user-attachments/assets/5c1c86ef-cfd1-4973-a29c-872c9c15346d)

旨在为 Pine Script 提供语法高亮功能。Pine Script 是 TradingView 平台上用于创建自定义技术指标和策略的脚本语言。

## Prettier - Code formatter

![image](https://github.com/user-attachments/assets/4e6f9c03-388a-43d8-a032-5c5943692268)

一个流行的代码格式化工具，支持多种编程语言，能够自动格式化代码以保持一致的风格。

## Pylance

![image](https://github.com/user-attachments/assets/decfe74d-0db9-4500-a2d0-9fa19b13b01f)

微软提供的 Python 语言服务器，提供高性能的语言支持，包括代码补全、类型检查等功能。

## Python

![image](https://github.com/user-attachments/assets/7adf9ea4-ac67-425a-ba3a-4aca67771254)

由微软提供，为 VS Code 提供全面的 Python 开发支持，包括代码补全、调试、单元测试等功能。

## RayThis: Instant Beautiful Code Screenshots

![image](https://github.com/user-attachments/assets/27f5d97f-9d4a-4a7d-ac55-9ea645a90c6b)

通过简化代码截图的流程，使得开发者可以更高效地生成和分享美观的代码图片，特别适合需要频繁分享代码片段的场景。

## Regex Previewer

![image](https://github.com/user-attachments/assets/f730e793-bf08-4946-9b56-530bc7625770)

实时预览正则表达式的匹配结果，支持多种编程语言。

## rust-analyzer

![image](https://github.com/user-attachments/assets/0cae23fe-c061-430a-85ad-ee8c8dec8747)

Rust 语言的一个高性能语言服务器，提供代码补全、类型检查等功能。

## Snazzy Operator

![image](https://github.com/user-attachments/assets/1a6cb192-7993-4985-8cb8-e48407fad637)

个人非常喜欢的一个主题！

## Solidity

![image](https://github.com/user-attachments/assets/a5a57777-36f9-4793-89d0-063ff586d957)

开发 Solidity 智能合约，提供代码补全、语法高亮等功能。

## Tailwind CSS IntelliSense

![image](https://github.com/user-attachments/assets/ced25631-2d40-4f35-a6f9-70977d0cb12a)

提供 Tailwind CSS 的智能提示和自动补全功能。

## TODO Highlight

![image](https://github.com/user-attachments/assets/baf35c05-2c11-412f-bc6c-096aea8fd47a)

高亮显示代码中的 TODO 和 FIXME 注释，便于跟踪和管理待办事项。

```json
# TODO: Add calculation logic here
# FIXME: Fix the bug in the following function
```

命令面板输入 `TODO Highlight: List highlighted annotations` 等命令。

## Trailing Spaces

![image](https://github.com/user-attachments/assets/bd666c8f-7043-4f2e-8251-81480b4bfcf1)

高亮显示和删除行尾的多余空格，保持代码整洁。

## Vim

![image](https://github.com/user-attachments/assets/fec8e795-2501-4c21-bc19-b53bd2235b0c)

提供了 Vim 模式的支持，使用户可以在 VS Code 中使用 Vim 的快捷键和编辑模式。

## vscode-icons (Mac 版)

![image](https://github.com/user-attachments/assets/c9d807b6-6b75-4162-8a96-f3372c5e9714)

提供了丰富的文件和文件夹图标，使文件管理更加直观和美观。

## YAML

![image](https://github.com/user-attachments/assets/700f69d2-b7e8-44d3-91be-07d9c13b6c79)

提供了 YAML 文件的语言支持，包括语法高亮、自动补全、格式校验和自动缩进等功能。

## Zig Language

![image](https://github.com/user-attachments/assets/39e83de9-c47d-4138-93fa-02a027f68642)

提供了 Zig 编程语言的支持，包括语法高亮、代码补全和基本的编译器检查功能。
