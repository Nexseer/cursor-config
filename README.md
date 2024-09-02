# cursor-config

👉 English | [简体中文](README_CN.md)

- [I. Introduction 💬](#i-introduction-)
- [II. Key Features 🌟](#ii-key-features-)
- [III. Pricing 💰](#iii-pricing-)
  - [Hobby (Free) Plan](#hobby-free-plan)
  - [Pro Plan ($20/month)](#pro-plan-20month)
  - [Business Plan ($40/month)](#business-plan-40month)
- [IV. Configuration 🛠️](#iv-configuration-️)
  - [1. Tips ⚙️](#1-tips-️)
  - [2. Custom Configuration ⛏️](#2-custom-configuration-️)
    - [Appearance Configuration](#appearance-configuration)
    - [Basic Settings](#basic-settings)
    - [Vim Mode Settings](#vim-mode-settings)
  - [3. Custom Key Bindings ⌨️](#3-custom-key-bindings-️)
  - [4. Key Bindings Overview 📚](#4-key-bindings-overview-)
    - [Search](#search)
    - [Navigation](#navigation)
    - [File Operations &amp; Explorer Panel](#file-operations--explorer-panel)
    - [Panel Operations](#panel-operations)
    - [Window Operations](#window-operations)
    - [Basic Operations](#basic-operations)
    - [Git Operations](#git-operations)
    - [Markdown Handling](#markdown-handling)
    - [Editing Operations](#editing-operations)
- [V. AI Features 💥](#v-ai-features-)
  - [1. Cursor Tab ✍️](#1-cursor-tab-️)
  - [2. Cursor Chat 💬](#2-cursor-chat-)
  - [3. Ctrl K ⛏️](#3-ctrl-k-️)
  - [4. Prompt Directory 📖](#4-prompt-directory-)
  - [5. Custom Rules 📐](#5-custom-rules-)
  - [6. Composer 💻](#6-composer-)
- [VI. Extensions 🔌](#vi-extensions-)
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
  - [filesize](#filesize)
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
  - [RayThis: Instant Beautiful Code Screenshots](#raythis-instant-beautiful-code-screenshots)
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

👉 [Cursor Website](https://www.trycursor.com/)

👉 [Cursor Forum](https://forum.cursor.com/)

👉 [Cursor Documents](https://docs.cursor.com/get-started/migrate-from-vscode)

> A code editor is typically a lightweight tool focused on editing source code, providing essential features like syntax highlighting, text editing, and file management. Code editors are often highly customizable and extensible, allowing users to add additional functionalities such as syntax checking and version control by installing plugins. Unlike Integrated Development Environments (IDEs), code editors are generally not tied to specific development frameworks or languages. Due to having fewer built-in features, they tend to be faster, with quicker startup times and lower system resource usage.

# I. Introduction 💬

> Built to make you extraordinarily productive, Cursor is the best way to code with AI.

Cursor is positioned as the AI code editor, aiming to assist developers in writing and editing code more efficiently through artificial intelligence. Cursor's integration with AI significantly boosts convenience and productivity, and the migration from VS Code is nearly seamless.

> Migrate VS Code Settings: Navigate to Cursor Settings (`ctrl shift j`) > General > Account

![image](https://github.com/user-attachments/assets/f10ffb9a-3e6a-4772-95fe-91832250bc9d)

Compared to GitHub Copilot, Cursor's standout feature is its powerful indexing capability. It can **build an index based on the entire project**, meaning that Cursor doesn't just offer simple code snippet completions but also deeply understands the structure and logic of the entire project. This global understanding enables Cursor to provide more accurate and project-specific code suggestions and completions.

When it comes to code refactoring, Cursor excels. It can easily handle basic refactoring tasks like renaming variables, moving files, and automatically updating references. Additionally, with AI assistance, Cursor can tackle more complex refactoring operations. For instance, it can intelligently suggest function relocation, parameter restructuring, and even code extraction and optimization. Cursor’s AI capabilities can also comprehend the developer's intent, offering context-aware suggestions and improvements, making advanced refactoring more intuitive and efficient.

# II. Key Features 🌟

👉 [Features | Cursor - The AI-first Code Editor](https://www.cursor.com/features#codebase-wide)

1. **Understand Your Codebase** - `Chat`: Users can query the codebase or reference specific files or documents directly through a chat interface. This is ideal for quick solutions or code reviews, and users can easily implement model-generated code snippets with a simple click.

2. **Copilot++** - `Tab`: With Cursor’s Copilot++ feature, pressing the Tab key allows the editor to predict and auto-complete code, recommending the next possible edits based on the context. This accelerates coding and improves efficiency, especially in handling complex code.

3. **Edit with Natural Language** - `Ctrl K`: Cursor’s `Ctrl K` feature lets users write and update code using natural language commands. For example, users can quickly execute complex programming tasks with simple prompts like “add a new method” or “update this function's parameters.”

4. **Comprehensive Ecosystem**: By leveraging the VS Code ecosystem, Cursor offers thousands of extensions for various programming languages, frameworks, tools, and functionalities, allowing users to easily find and install extensions to meet specific needs.

# III. Pricing 💰

👉 [Pricing | Cursor](https://www.trycursor.com/pricing)

🎉 Two weeks of Pro trial!

## Hobby (Free) Plan

- 2000 completions per month.
- 50 slow premium requests.
- 100 uses of the Cursor-small model.

## Pro Plan ($20/month)

- All Hobby plan features.
- Unlimited completions.
- 500 fast premium requests (includes GPT-4, GPT-4o, and Claude 3.5 Sonnet).
- Unlimited slow premium requests.
- Unlimited Cursor-small usage.
- 10 Claude Opus uses per day.

## Business Plan ($40/month)

- All Pro plan features.
- Centralized billing, admin usage dashboards, enforced privacy mode, and zero data retention policies by OpenAI/Anthropic. Privacy mode ensures code is only stored on the user's device, with no use for training purposes.

# IV. Configuration 🛠️

## 1. Tips ⚙️

- **Disable Auto-Save**: While auto-save can prevent data loss, frequent saves may increase system I/O load, especially in large or complex projects, potentially slowing down the editor.

- **Auto-Generate Git Commit Messages**: Use `ctrl l` to enter the AI Chat panel, input `@Commit (Diff of Working State)` to get changes, then prompt `give me a one-line commit message`.

- **Codebase Indexing Ignoration**: Open Cursor Settings with `ctrl shift j`, or add `.cursorignore` to your project to exclude specific files and directories from being indexed, improving performance and search efficiency.

![image](https://github.com/user-attachments/assets/ee4a1a68-7ce6-439f-a395-2640c0fe8bf9)

## 2. Custom Configuration ⛏️

To open the settings, you can use the following methods:

1. Shortcut: `ctrl ,`
2. Open the Command Palette: `ctrl shift p` and type `Open VS Code Settings`

> The settings panel offers a user-friendly graphical interface where users can modify configurations by clicking and selecting options, without the need to directly edit the JSON file.

For more flexibility and fine-tuned control, we choose to use the `settings.json` file.

![image](https://github.com/user-attachments/assets/15389db1-d017-42fd-b767-b8e0d98e5cbc)

### Appearance Configuration

```json
// Set the window zoom level to 1, which means the interface is zoomed to 110%
"window.zoomLevel": 1,
// Display vertically
"workbench.activityBar.orientation": "vertical",
// Theme configuration
"workbench.colorTheme": "Snazzy Operator",
// Set the icon theme
"workbench.iconTheme": "vscode-icons-mac",
// Enable smooth scrolling
"workbench.list.smoothScrolling": true,
// Set the font size for the chat editor
"chat.editor.fontSize": 18,
// Disable compact display mode for folders
"explorer.compactFolders": false,
// Set the editor font size
"editor.fontSize": 24,
// Set the editor font family
"editor.fontFamily": "Cascadia Code NF",
// Set the font family for inlay hints
"editor.inlayHints.fontFamily": "Consolas",
// Enable minimap in the editor
"editor.minimap.enabled": true,
// Automatically format the code on save
"editor.formatOnSave": true,
// Use relative line numbers
"editor.lineNumbers": "relative",
// Keep 6 lines above and below the cursor always visible
"editor.cursorSurroundingLines": 6,
// Enable smooth caret animation
"editor.cursorSmoothCaretAnimation": "on",
// Enable active bracket pair guides
"editor.guides.bracketPairs": "active",
// Automatically insert closing brackets
"editor.autoClosingBrackets": "always",
// Enable sticky hover effects
"editor.hover.sticky": true,
// Enable sticky scrolling
"editor.stickyScroll.enabled": true,
// Set the terminal font size
"terminal.integrated.fontSize": 16,
// Set the terminal font family
"terminal.integrated.fontFamily": "Cascadia Code NF",
```

### Basic Settings

```json
// Do not restore any previously opened windows on restart
"window.restoreWindows": "none",
// Disable font size zooming with the mouse wheel in the editor
"editor.mouseWheelZoom": false,
// Automatically run ESLint's `fixAll` action on save to fix all auto-fixable issues
"editor.codeActionsOnSave": {
  "source.fixAll.eslint": "explicit"
},
// Associate .mdx files with the markdown file type
"files.associations": {
  "*.mdx": "markdown"
},
// Trim trailing whitespace on save
"files.trimTrailingWhitespace": true,
// Do not show recommended extensions
"extensions.ignoreRecommendations": true,
// Set Prettier as the default code formatter
"editor.defaultFormatter": "esbenp.prettier-vscode",
// Configure Prettier to use single quotes instead of double quotes
"prettier.singleQuote": true,
// Language-specific formatter settings
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
// Exclude specific files and folders from search
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
// File patterns to exclude during file scanning
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
]
```

### Vim Mode Settings

The vscode-vim extension comes with several built-in plugins that allow for quick operations.

- **Easymotion Plugin**: With the key combination `<leader><leader>s<char>`, you can quickly navigate to any line you want to edit, enhancing navigation efficiency.

- **vim-commentary Plugin**: `gc` in visual mode and `gcc` in normal mode toggle comments.

- **vim-surround Plugin**: This plugin allows you to modify or delete surrounding quotes easily:

```vim
ds<existing>
cs<existing><desired>

# Example: Remove []
[1, 2, 3] -> ds[

# Example: Change [] to ()
[1, 2, 3] -> cs[(
```

```json
// Set the Vim leader key to space
"vim.leader": "<space>",
// Enable the EasyMotion plugin
"vim.easymotion": true,
// Allow Vim to use the system clipboard
"vim.useSystemClipboard": true,
// Non-recursive key bindings in normal mode
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
// Insert Mode Key Bindings
"vim.insertModeKeyBindings": [],
// Command Mode Non-Recursive Key Bindings
"vim.commandLineModeKeyBindingsNonRecursive": [],
"vim.handleKeys": {
  "<C-a>": false
}
```

> 📕 Non-recursive key bindings: ensures that when a key combination is pressed, only the command directly associated with it will be executed, and no other key bindings will be triggered.

## 3. Custom Key Bindings ⌨️

To open the key bindings settings, you can use the following methods:

1. Shortcut: `ctrl shift k`
2. Open the Command Palette: `ctrl shift p` and type `Preferences: Open Keyboard Shortcuts`
3. Open the Command Palette: `ctrl shift p` and type `Preferences: Open Default Keyboard Shortcuts (JSON)`

> The keybindings panel provides a user-friendly graphical interface where users can modify configurations by clicking and selecting options, without needing to directly edit the JSON file. It also allows you to view configurable key functions, and you can copy the Command ID.

For more flexibility and fine-tuned control, we choose to use the `keybindings.json` file.

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
    "key": "a",
    "command": "explorer.newFile",
    "when": " explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus "
  },
  {
    "key": "A",
    "command": "explorer.newFolder",
    "when": " explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus "
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

## 4. Key Bindings Overview 📚

### Search

| Key Binding    | Function               |
| -------------- | ---------------------- |
| `ctrl shift f` | Universal search       |
| `/` or `?`     | Search                 |
| `n`            | Next search result     |
| `N`            | Previous search result |

### Navigation

| Key Binding | Function                                         |
| ----------- | ------------------------------------------------ |
| `g d`       | Jump to definition                               |
| `g D`       | Jump to declaration                              |
| `g r`       | Jump to references                               |
| `g i`       | Jump to implementation                           |
| `g b`       | Go back to previous cursor position              |
| `g h`       | Move cursor to the beginning of the current line |
| `g l`       | Move cursor to the end of the current line       |

### File Operations & Explorer Panel

| Key Binding  | Function               |
| ------------ | ---------------------- |
| `<leader> e` | Open file explorer     |
| `a`          | Create a new file      |
| `A`          | Create a new directory |
| `c`          | Copy                   |
| `d`          | Delete                 |
| `p`          | Paste                  |
| `r`          | Rename                 |
| `x`          | Cut                    |

### Panel Operations

| Key Binding   | Function                               |
| ------------- | -------------------------------------- |
| `ctrl t`      | Toggle terminal                        |
| `<space> p d` | Show problems (e.g., errors, warnings) |
| `<space> p o` | Show output                            |
| `ctrl w`      | Close panel                            |

### Window Operations

| Key Binding   | Function                 |
| ------------- | ------------------------ |
| `<space> w c` | Close all tabs           |
| `<space> w k` | Split panel upwards      |
| `<space> w j` | Split panel downwards    |
| `<space> w h` | Split panel to the left  |
| `<space> w l` | Split panel to the right |

### Basic Operations

| Key Binding    | Function                         |
| -------------- | -------------------------------- |
| `ctrl alt n`   | Run (Code Runner)                |
| `H`            | Previous tab                     |
| `L`            | Next tab                         |
| `K`            | Show hover information           |
| `<space> c f`  | Format code                      |
| `<space> c r`  | Rename                           |
| `<leader> f f` | Open file or folder              |
| `<space> f o`  | Find file outline                |
| `<space> f p`  | Open recent project              |
| `<space> f q`  | Quick open a file in the project |
| `ctrl shift p` | Command Palette                  |
| `ctrl shift d` | Run and Debug                    |
| `ctrl shift k` | Keyboard Shortcuts               |
| `ctrl shift x` | Extensions                       |
| `F11`          | Toggle full-screen mode          |

### Git Operations

| Key Binding   | Function                                |
| ------------- | --------------------------------------- |
| `<space> g [` | Jump to the previous Git change         |
| `<space> g ]` | Jump to the next Git change             |
| `<space> g b` | Toggle `git blame`                      |
| `<space> g d` | Toggle diff view for the current `hunk` |
| `<space> g r` | Revert selected `hunks`                 |

### Markdown Handling

| Key Binding   | Function                                |
| ------------- | --------------------------------------- |
| `<space> m o` | Open Markdown preview                   |
| `<space> m p` | Open Markdown preview in the side panel |

### Editing Operations

| Key Binding | Function       |
| ----------- | -------------- |
| `ctrl a`    | Select all     |
| `ctrl w`    | Close tab      |
| `ctrl y`    | Redo           |
| `alt up`    | Move line up   |
| `alt down`  | Move line down |

# V. AI Features 💥

## 1. Cursor Tab ✍️

Cursor Tab is a core feature of the Cursor editor, offering more than just code completion—it provides a **broader range of "editing"** capabilities.

1. **Auto-complete Code**
   Press `Tab` at the cursor position, and Cursor Tab will suggest completions based on the context. Press `Tab` again to accept the suggestion, and Cursor Tab may automatically complete the code.

2. **Multi-line Editing**
   Modify multiple lines at once, eliminating the need to repeatedly trigger completions.

3. **Fix Linter Errors**
   Offers suggestions based on your recent changes and linter errors.

4. **Predict Next Edit**
   Automatically jump to the next relevant change. For example, if you add a type annotation to a function, the model can quickly infer that you intend to add type annotations to other functions in the file, and pressing `Tab` will take you to the next suggested change.

5. **AI-assisted Refactoring**
   Automatically generates and applies editing changes.

**How to Use:**

- Accept Suggestion: Press `Tab`
- Reject Suggestion: Press `Esc` or continue typing
- Accept Suggestions Character by Character: Press `Ctrl/⌘ →`

## 2. Cursor Chat 💬

Cursor Chat is a chat interface powered by large language model (LLM) technology that allows users to interact with AI through conversation. It can answer programming-related questions, generate code, fix errors, optimize code, and more, automatically incorporating the context of the entire codebase. You can use the `@` operator to flexibly specify context. 👉 See more details at [Cursor @ Symbols](https://docs.cursor.com/context/@-symbols/basic).

**How to Use:**

- Open AI Panel: Press `Ctrl/⌘ L`
- Enter Questions or Requests: Type in the input box and press `Enter`

## 3. Ctrl K ⛏️

`Ctrl K` is a shortcut in the Cursor editor used to invoke the AI assistant for code generation and editing. It can automatically generate code, complete code, fix errors, optimize code, and more, greatly enhancing development efficiency. This also applies to terminals, providing functionality similar to Wrap AI.

1. Code Generation
2. Bug Detection and Fixing
3. Code Explanation
4. Documentation Generation
5. Code Optimization Suggestions
   ...

**How to Use:**

- Press `Ctrl/⌘ K` to open the prompt bar
- Use the `@` symbol to reference other contexts
- Enter a command and press `Enter`

You can also select a block of code, press `Ctrl/⌘ K`, directly input your request or question, and let the AI assist you. Green code blocks indicate AI-generated code, while red code blocks indicate the original code to be replaced.

## 4. Prompt Directory 📖

[Cursor Directory](https://cursor.directory/) is an open-source resource hub specifically designed for the Cursor editor. It provides and collects various configuration files and a series of prompts. These prompts help the Cursor editor better understand the developer's intent, leading to more accurate code completion, error fixing, and other intelligent editing features.

## 5. Custom Rules 📐

Add custom rules to Cursor, such as **global rules** or **project-specific rules**, which will apply to features like `Cursor Chat` and `Ctrl/⌘ K`.

**How to Use:**

- Global Rules: Go to Cursor Settings > General > AI Rules

![image](https://github.com/user-attachments/assets/69168aa6-9522-44c4-a70b-a0d5c85cb8fe)

- Project-specific rules: Create a `.cursorrules` file in the project root directory and add the appropriate rules.

## 6. Composer 💻

Composer is a multi-file editing tool designed to handle complex programming tasks. It goes beyond single-line or single-file code generation by enabling editing and creation across multiple files.

Composer assists developers in completing complex programming tasks more efficiently, whether it's generating new code, optimizing existing code, or creating entire applications. Composer provides robust support throughout the development process.

**How to Use:**

- Ensure the feature is enabled.

![image](https://github.com/user-attachments/assets/7e4dfa33-197b-4d6c-b7d1-3ea32e0739a2)

- Press `Ctrl/⌘ Shift I` to open it.

# VI. Extensions 🔌

## Auto Close Tag

![image](https://github.com/user-attachments/assets/c9e8c7de-e23f-4fe0-bcf5-6a162ebe76f5)

Automatically closes HTML, XML, and JSX tags, reducing manual input.

## Auto Import

![image](https://github.com/user-attachments/assets/ca730c98-f917-42cf-98c5-0a23160d2c51)

Automatically imports modules or libraries, reducing the need to manually write import statements.

## Auto Rename Tag

![image](https://github.com/user-attachments/assets/23d078de-ce9b-49cb-b979-fc5447ee75b4)

Synchronizes changes between the opening and closing HTML/XML tags to ensure consistency.

## C/C++

![image](https://github.com/user-attachments/assets/dc1426ec-1a17-4283-a8de-af08c4820a12)

Provides cross-platform support for C and C++ development in VS Code, including code completion (IntelliSense), debugging, and code navigation.

## Cairo 1.0

![image](https://github.com/user-attachments/assets/82b43fc9-5758-4b50-a01a-7f606b3381c0)

Adds support for the Cairo programming language.

## Clang-Format

![image](https://github.com/user-attachments/assets/4ee48d97-8da5-49f8-b810-88d9f876e242)

Significantly enhances code cleanliness and consistency, improving development efficiency and code quality.

## Code Runner

![image](https://github.com/user-attachments/assets/ab0ce013-52ac-4b3c-9376-02420302f530)

Supports running code snippets or entire files in multiple programming languages.

## Database Client JDBC

![image](https://github.com/user-attachments/assets/3b5293c3-a934-4ad0-94e4-ff381eec4adf)

Manages and connects various databases within VS Code, including MySQL, PostgreSQL, SQLite, Redis, ClickHouse, and others, with support for JDBC connections.

## DotENV

![image](https://github.com/user-attachments/assets/6db4dc44-fd12-4395-b25a-bf6a6ea09b13)

Handles `.env` files in VS Code, offering syntax highlighting and auto-completion features.

## ES7 React/Redux/GraphQL/React-Native snippets

![image](https://github.com/user-attachments/assets/e3a0292c-e68a-48bb-8af6-b710f71897ff)

Provides a set of code snippets to quickly write React, Redux, GraphQL, and React-Native code.

## ESLint

![image](https://github.com/user-attachments/assets/6b1a272f-7194-4f2a-896a-26c9c0f1fc85)

Helps developers adhere to consistent coding styles when writing JavaScript and TypeScript, and automatically detects and fixes issues in the code.

## Even Better TOML

![image](https://github.com/user-attachments/assets/88022129-8b6b-4600-b60e-68752364a2ef)

Provides syntax highlighting and validation for TOML files.

## filesize

![image](https://github.com/user-attachments/assets/5664864d-3f4b-46a6-92e5-a31b91ed8fe0)

Displays the current file's size in the status bar. Clicking on the file size information in the status bar also provides detailed file information (e.g., creation time, modification time), which is useful for managing project files and optimizing file size.

## GitLens — Git supercharged

![image](https://github.com/user-attachments/assets/3e0eae7a-965a-4710-9d0b-7b89234e7798)

Enhances Git capabilities, making version control more convenient for developers.

## Image Preview

![image](https://github.com/user-attachments/assets/740f473c-8b22-4bce-adef-520b348fdccd)

Allows viewing images directly within the editor.

## Live Server

![image](https://github.com/user-attachments/assets/c78b62f1-9f5f-4c1d-9db1-d4a7c5c0ac56)

Launches a local development server that automatically refreshes the browser when files are saved, greatly improving development efficiency.

## Markdown Preview Enhanced

![image](https://github.com/user-attachments/assets/b1531b6e-4219-4bc3-af17-1ef3e3a9b652)

Significantly enhances the editing and previewing experience for Markdown files, with the option to export them as PDFs.

## Mojo 🔥

![image](https://github.com/user-attachments/assets/60471bde-0c41-4060-b3a4-41d42cbc62b7)

Adds support for the Mojo programming language, including syntax highlighting and code completion.

## MySQL

![image](https://github.com/user-attachments/assets/44437977-737e-4d7e-81fc-4254a23892b7)

Manages and connects to MySQL databases, offering features like database browsing and query execution.

## Npm Intellisense

![image](https://github.com/user-attachments/assets/6cdef421-767a-4e0c-af3d-fee315ddf8a2)

Simplifies the process of importing npm modules by providing auto-completion for import statements.

## Path Intellisense

![image](https://github.com/user-attachments/assets/51c4bf3f-5c65-4e21-8c96-237f74c97ece)

Provides auto-completion for file paths, supporting various programming languages.

## Pine Script Syntax Highlighter

![image](https://github.com/user-attachments/assets/5c1c86ef-cfd1-4973-a29c-872c9c15346d)

Provides syntax highlighting for Pine Script, the scripting language used on the TradingView platform to create custom technical indicators and strategies.

## Prettier - Code formatter

![image](https://github.com/user-attachments/assets/4e6f9c03-388a-43d8-a032-5c5943692268)

A popular code formatting tool that supports multiple programming languages and automatically formats code to maintain a consistent style.

## Pylance

![image](https://github.com/user-attachments/assets/decfe74d-0db9-4500-a2d0-9fa19b13b01f)

A high-performance language server provided by Microsoft for Python, offering features like code completion and type checking.

## Python

![image](https://github.com/user-attachments/assets/7adf9ea4-ac67-425a-ba3a-4aca67771254)

A comprehensive support extension provided by Microsoft for Python development in VS Code, including code completion, debugging, unit testing, and more.

## RayThis: Instant Beautiful Code Screenshots

![image](https://github.com/user-attachments/assets/27f5d97f-9d4a-4a7d-ac55-9ea645a90c6b)

Simplifies the process of taking code screenshots, making it easier for developers to generate and share visually appealing code images, especially useful in scenarios that require frequent code snippet sharing.

## Regex Previewer

![image](https://github.com/user-attachments/assets/f730e793-bf08-4946-9b56-530bc7625770)

Provides real-time preview of regex matches, supporting multiple programming languages.

## rust-analyzer

![image](https://github.com/user-attachments/assets/0cae23fe-c061-430a-85ad-ee8c8dec8747)

A high-performance language server for Rust, providing code completion and type checking.

## Snazzy Operator

![image](https://github.com/user-attachments/assets/1a6cb192-7993-4985-8cb8-e48407fad637)

A personal favorite theme for the editor.

## Solidity

![image](https://github.com/user-attachments/assets/a5a57777-36f9-4793-89d0-063ff586d957)

Supports Solidity smart contract development with features like code completion and syntax highlighting.

## Tailwind CSS IntelliSense

![image](https://github.com/user-attachments/assets/ced25631-2d40-4f35-a6f9-70977d0cb12a)

Provides intelligent suggestions and auto-completion for Tailwind CSS.

## TODO Highlight

![image](https://github.com/user-attachments/assets/baf35c05-2c11-412f-bc6c-096aea8fd47a)

Highlights `TODO` and `FIXME` comments in the code, making it easier to track and manage tasks.

```json
# TODO: Add calculation logic here
# FIXME: Fix the bug in the following function
```

Use the command `TODO Highlight: List highlighted annotations` in the command palette.

## Trailing Spaces

![image](https://github.com/user-attachments/assets/bd666c8f-7043-4f2e-8251-81480b4bfcf1)

Highlights and removes trailing whitespace in the code, keeping it clean.

## Vim

![image](https://github.com/user-attachments/assets/fec8e795-2501-4c21-bc19-b53bd2235b0c)

Brings Vim mode support to VS Code, allowing users to use Vim's key bindings and editing modes.

## vscode-icons (Mac 版)

![image](https://github.com/user-attachments/assets/c9d807b6-6b75-4162-8a96-f3372c5e9714)

Provides rich file and folder icons, making file management more intuitive and visually appealing.

## YAML

![image](https://github.com/user-attachments/assets/700f69d2-b7e8-44d3-91be-07d9c13b6c79)

Adds language support for YAML files, including syntax highlighting, auto-completion, format validation, and auto-indentation.

## Zig Language

![image](https://github.com/user-attachments/assets/39e83de9-c47d-4138-93fa-02a027f68642)

Adds support for the Zig programming language, including syntax highlighting, code completion, and basic compiler checks.
