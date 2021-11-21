<h3 align="center">👋 Hi! This is my vscode configuration</h3>
<p align="center">
  <a href="https://gael-lopes-da-silva.github.io/MyPortfolio/">Website</a>
</p>

---

<p align="center">🔌 I just want to share my working environment, so here is my vscode configuration. I have tried other editors by the past like Sublim Text, Atome, and Neovim but I finaly switched to vscode.</p>

<p align="center">⚙️ I use the vim keybindings, so if you don't want to use it or if you don't know to use it and just want to use normal vscode keybindings, just diseable the vim extension.</p>

---

### Screenshots
![](screenshots/Screenshot1.png)
![](screenshots/Screenshot2.png)

### Font
- [Cascadia Code](https://github.com/microsoft/cascadia-code)

### Extensions
- [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
- [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
- [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
- [Jupyter Keymap](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter-keymap)
- [Jupyter Notebook Renderers](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter-renderers)
- [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)
- [Markdown Emoji](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-emoji)
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
- [Monokai Accents](https://marketplace.visualstudio.com/items?itemName=tw.monokai-accent)
- [Nim](https://marketplace.visualstudio.com/items?itemName=nimsaem.nimvscode)
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
- [Visual Studio IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)

### Settings
~~~json with comments
{
  // options
  "editor.suggestSelection": "first",
  "editor.suggest.preview": true,
  "editor.suggest.showIcons": true,
  "editor.suggest.showFiles": true,
  "editor.suggest.showFolders": true,
  "editor.autoIndent": "full",
  "editor.autoClosingBrackets": "always",
  "editor.quickSuggestionsDelay": 0,
  "editor.linkedEditing": false,
  "editor.folding": true,
  "editor.foldingHighlight": false,
  "editor.foldingStrategy": "auto",
  "explorer.confirmDelete": false,
  "extensions.ignoreRecommendations": true,
  "files.insertFinalNewline": true,
  "files.autoSave": "afterDelay",
  "files.enableTrash": true,
  "files.encoding": "utf8",
  "files.restoreUndoStack": true,
  "security.workspace.trust.enabled": false,
  "debug.openDebug": "neverOpen",
  "debug.terminal.clearBeforeReusing": true,
  "workbench.editor.enablePreview": false,
  "workbench.activityBar.visible": false,
  "workbench.editorAssociations": {
    "*.ipynb": "jupyter-notebook",
    "*.nims": "nimscript"
  },

  // appearance
  "window.title": "${dirty}${activeEditorShort}${separator}${appName}",
  "editor.cursorWidth": 3,
  "editor.lineHeight": 24,
  "editor.fontSize": 17,
  "editor.fontFamily": "Cascadia Code, monospace",
  "editor.codeLensFontFamily": "Cascadia Code, monospace",
  "editor.fontLigatures": true,
  "editor.cursorBlinking": "solid",
  "editor.renderWhitespace": "selection",
  "editor.matchBrackets": "never",
  "editor.wordWrap": "on",
  "editor.overviewRulerBorder": false,
  "editor.hideCursorInOverviewRuler": true,
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  "editor.padding.bottom": 1,
  "editor.padding.top": 1,
  "editor.lineNumbers": "relative",
  "editor.renderLineHighlight": "all",
  "editor.minimap.enabled": false,
  "breadcrumbs.enabled": false,
  "explorer.compactFolders": false,
  "workbench.editor.tabCloseButton": "off",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Monokai +Blue",

  // synchronization
  "settingsSync.ignoredSettings": [
    "-window.zoomLevel"
  ],

  // extensions
  "errorLens.gutterIconsEnabled": true,
  "errorLens.delay": 1,
  "errorLens.followCursor": "closestProblem",
  "errorLens.fontFamily": "Cascadia Code, monospace",
  "git.autofetch": true,
  "git.enableSmartCommit": true,
  "git.confirmSync": false,
  "jupyter.askForKernelRestart": false,
  "notebook.lineNumbers": "on",
  "nim.enableNimsuggest": true,
  "nim.lintOnSave": true,
  "vim.useSystemClipboard": true,
  "vim.cursorStylePerMode.visual": "",
  "vim.cursorStylePerMode.normal": "block",
  "vim.cursorStylePerMode.insert": "line",
  "vim.handleKeys": {
    "<C-c>": false,
    "<C-v>": false,
    "<C-x>": false,
    "<C-w>": false,
    "<C-b>": false,
    "<C-z>": false,
    "<C-y>": false,
  },
  "code-runner.clearPreviousOutput": true,
  "code-runner.ignoreSelection": true,
  "code-runner.runInTerminal": false,
  "code-runner.fileDirectoryAsCwd": true,
  "code-runner.preserveFocus": true,
  "code-runner.executorMap": {
    "java": "javac $fileName && java $fileNameWithoutExt",
    "c": "gcc $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
    "cpp": "g++ $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
    "python": "python -u $fileName",
    "powershell": "powershell -ExecutionPolicy ByPass -File",
    "bat": "powershell",
    "shellscript": "powershell",
    "csharp": "dotnet run",
    "nim": "nim c -r --verbosity:2 --hints:off $fileName",
    "makefile": "mingw32-make -f",
  },
  
  // temporary
  "window.zoomLevel": 1,
}
~~~

### Keybindings
~~~json with comments
[
    {
        "key": "f5",
        "command": "code-runner.run"
    },
    {
        "key": "ctrl+f5",
        "command": "code-runner.stop"
    },
    {
        "key": "tab",
        "command": "editor.action.indentLines",
        "when": "editorTextFocus && !editorTabMovesFicus"
    },
    {
        "key": "shift+tab",
        "command": "outdent",
        "when": "editorTextFocus && !editorTabMovesFicus"
    },
    {
        "key": "ctrl+j",
        "command": "selectNextSuggestion",
        "when": "suggestWidgetMultipleSuggestions && suggestWidgetVisible && textInputFocus"
    },
    {
        "key": "ctrl+k",
        "command": "selectPrevSuggestion",
        "when": "suggestWidgetMultipleSuggestions && suggestWidgetVisible && textInputFocus"
    }
]
~~~
