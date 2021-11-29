<h3 align="center">👋 Hi! This is my vscode configuration</h3>
<p align="center">
  <a href="https://gael-lopes-da-silva.github.io/MyPortfolio/">Website</a>
</p>

---

<p align="center">🔌 I just want to share my working environment, so here is my vscode configuration. I have tried other editors by the past like Sublim Text, Atome, and Neovim but I finaly switched to vscode.</p>

<p align="center">⚙️ I use the emacs keybindings, so if you don't want to use it or if you don't know how to use it and you just want to use normal vscode keybindings, diseable the vim extension.</p>

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
- [Emacs](https://marketplace.visualstudio.com/items?itemName=vscodeemacs.emacs)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
- [Monokai Accents](https://marketplace.visualstudio.com/items?itemName=tw.monokai-accent)
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
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
  "files.defaultLanguage": "${activeEditorLanguage}",
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
  
  // appearance
  "window.menuBarVisibility": "hidden",
  "window.title": "${dirty}${activeEditorShort}${separator}${appName}",
  "editor.cursorWidth": 3,
  "editor.lineHeight": 24,
  "editor.fontSize": 17,
  "editor.fontFamily": "Cascadia Code, monospace",
  "editor.codeLensFontFamily": "Cascadia Code, monospace",
  "editor.fontLigatures": true,
  "editor.cursorStyle": "block",
  "editor.cursorBlinking": "solid",
  "editor.renderWhitespace": "selection",
  "editor.matchBrackets": "never",
  "editor.wordWrap": "on",
  "editor.guides.indentation": false,
  "editor.guides.bracketPairs": false,
  "editor.overviewRulerBorder": false,
  "editor.hideCursorInOverviewRuler": true,
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  "editor.padding.bottom": 1,
  "editor.padding.top": 1,
  "editor.lineNumbers": "relative",
  "editor.renderLineHighlight": "all",
  "editor.minimap.enabled": false,
  "explorer.compactFolders": false,
  "breadcrumbs.enabled": false,
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Monokai +Blue",
  "workbench.colorCustomizations": {
    "editorError.foreground":   "#00000000",
    "editorWarning.foreground": "#00000000",
    "editorInfo.foreground":    "#00000000",
    "editorCursor.foreground": "#ffd900",
    "editorLineNumber.activeForeground": "#ffd900"
  },

  // synchronization
  "settingsSync.ignoredSettings": [
    "-window.zoomLevel"
  ],
  
  // extensions
  "C_Cpp.autoAddFileAssociations": false,
  "errorLens.gutterIconsEnabled": true,
  "errorLens.enabledDiagnosticLevels": [
    "error",
    "info"
  ],
  "errorLens.delay": 1,
  "errorLens.followCursor": "closestProblem",
  "errorLens.fontFamily": "Cascadia Code, monospace",
  "git.autofetch": true,
  "git.enableSmartCommit": true,
  "git.confirmSync": false,
  "notebook.lineNumbers": "on",
  "code-runner.clearPreviousOutput": true,
  "code-runner.ignoreSelection": true,
  "code-runner.runInTerminal": false,
  "code-runner.fileDirectoryAsCwd": true,
  "code-runner.preserveFocus": true,
  "code-runner.executorMap": {
    "java": "javac $fileName && java $fileNameWithoutExt",
    "cpp": "clang++ -o $fileNameWithoutExt $fileName && $fileNameWithoutExt",
    "c": "clang -o $fileNameWithoutExt $fileName && $fileNameWithoutExt",
    "shellscript": "bash $fileName",
    "python": "python $fileName",
  },
  "better-comments.multilineComments": true,
  "better-comments.tags": [
    // todo
    {
      "tag": "todo",
      "color": "#FFB900",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": true,
      "italic": false
    },

    // fixme
    {
      "tag": "fixme",
      "color": "#FF2200",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": true,
      "italic": false
    },
    
    // note
    {
      "tag": "note",
      "color": "#48E338",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": true,
      "italic": false
    },
  
    // review
    {
      "tag": "review",
      "color": "#0095FF",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": true,
      "italic": false
    },

    // deprecated
    {
      "tag": "deprecated",
      "color": "#505050",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": true,
      "italic": false
    },

    // hack
    {
      "tag": "hack",
      "color": "#CA90E0",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": true,
      "italic": false
    },
  ],

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
]
~~~
