<h3 align="center">Visual studio code configuration</h3>

---

<p align="center">⚙️ I use emacs keybindings, so if you don't want to use it or if you don't know how to use it you can diseable the emacs extension.</p>

---

### 🖼️ Screenshots
![](screenshots/Screenshot1.png)
![](screenshots/Screenshot2.png)

### 📃 Font
- [Cascadia Code](https://github.com/microsoft/cascadia-code)

### ⚙️ Extensions
- [Awesome Emacs Keymap](https://marketplace.visualstudio.com/items?itemName=tuttieee.emacs-mcx)
- [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
- [C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp)
- [Command Runner](https://marketplace.visualstudio.com/items?itemName=edonet.vscode-command-runner)
- [dotnet](https://marketplace.visualstudio.com/items?itemName=leo-labs.dotnet)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
- [Material Product Icons](https://marketplace.visualstudio.com/items?itemName=PKief.material-product-icons)
- [Monokai Accents](https://marketplace.visualstudio.com/items?itemName=tw.monokai-accent)
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)
- [Visual Studio IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)

### 🔧 Settings
~~~json with comments
{
  // options
  "editor.suggestSelection": "first",
  "editor.suggest.preview": true,
  "editor.autoIndent": "full",
  "editor.detectIndentation": false,
  "editor.autoClosingBrackets": "always",
  "editor.quickSuggestionsDelay": 0,
  "editor.linkedEditing": false,
  "editor.folding": true,
  "editor.foldingHighlight": false,
  "editor.foldingStrategy": "auto",
  "editor.autoClosingQuotes": "always",
  "editor.codeLens": true,
  "editor.colorDecorators": true,
  "editor.definitionLinkOpensInPeek": true,
  "editor.dragAndDrop": false,
  "editor.emptySelectionClipboard": true,
  "editor.fastScrollSensitivity": 5,
  "editor.largeFileOptimizations": true,
  "editor.lightbulb.enabled": false,
  "editor.links": true,
  "editor.mouseWheelZoom": true,
  "editor.unicodeHighlight.invisibleCharacters": false,
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
  "diffEditor.codeLens": true,
  "diffEditor.wordWrap": "inherit",
  
  // appearance
  "window.menuBarVisibility": "hidden",
  "window.zoomLevel": 1,
  "window.dialogStyle": "custom",
  "window.titleBarStyle": "custom",
  "window.title": "${dirty}${activeEditorShort}${separator}${appName}",
  "editor.cursorWidth": 3,
  "editor.lineHeight": 21,
  "editor.fontSize": 18,
  "editor.fontFamily": "Cascadia Code, monospace",
  "editor.codeLensFontFamily": "Cascadia Code, monospace",
  "editor.cursorStyle": "block",
  "editor.cursorBlinking": "solid",
  "editor.renderWhitespace": "selection",
  "editor.matchBrackets": "always",
  "editor.wordWrap": "bounded",
  "editor.wordWrapColumn": 150,
  "editor.wrappingIndent": "same",
  "editor.wrappingStrategy": "simple",
  "editor.guides.indentation": true,
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
  "workbench.productIconTheme": "material-product-icons",
  "terminal.integrated.fontFamily": "Cascadia Code, monospace",
  "terminal.integrated.customGlyphs": true,
  "terminal.integrated.gpuAcceleration": "on",
  
  // custom theming
  "workbench.colorCustomizations": {
    "editorError.foreground": "#00000000",
    "editorWarning.foreground": "#00000000",
    "editorInfo.foreground": "#00000000",
    "editorCursor.foreground": "#ffd900",
    "editorLineNumber.activeForeground": "#ffd900",
    "editorLink.activeForeground": "#ffffff"
  },
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": [
          "",
          "entity.name.function",
          "support.function",
          "support.type.property-name.json",
          "constant.language",
          "entity.other.attribute-name",
          "storage",
          "variable.parameter",
          "variable.other.object",
          "markup.underline.link.markdown",
          "markup.raw.block.markdown",
          "markup.heading.markdown",
          "support.type",
          "variable.other.constant",
          "support.class",
          "support.type.property-name.css",
          "support.constant",
          "support.function",
          "entity.name.variable.parameter",
          "entity.name.type.namespace.cs",
          "entity.name.type.class.cs",
          "entity.name.type.class.java",
        ],
        "settings": {
          "foreground": "#ffffff"
        }
      },
      {
        "scope": [
          "keyword",
          "storage.type",
          "keyword.operator",
          "entity.name.tag",
          "meta.separator.markdown",
          "punctuation.definition.list",
          "constant.numeric",
          "keyword.operator.logical",
          "entity.name.type",
          "punctuation.definition.bold.markdown",
          "punctuation.definition.italic.markdown",
          "punctuation.definition.raw.markdown",
          "markup.fenced_code.block.markdown",
          "punctuation.definition.heading.markdown",
          "markup.quote.markdown",
          "storage.modifier.cs",
          "storage.modifier.java",
          "support.function.builtin.shell",
        ],
        "settings": {
          "foreground": "#ffd900"
        }
      },
      {
        "scope": [
          "string",
          "markup.inline.raw.string.markdown",
          "entity.other.attribute-name.pseudo-element.css",
          "entity.other.attribute-name.pseudo-class.css",
        ],
        "settings": {
          "foreground": "#378b1d"
        }
      },
      {
        "scope": [
          "punctuation.definition.string.begin",
          "punctuation.definition.string.end",
          "punctuation.definition.char.begin.cs",
          "punctuation.definition.char.end.cs",
          "comment",
        ],
        "settings": {
          "foreground": "#6b6b6b"
        }
      }
    ]
  },
  "editor.semanticTokenColorCustomizations": {
    "rules": {
      "keyword": "#ffd900",
      "string": "#378b1d",
      "type": "#ffffff",
      "parameter": "#ffffff",
      "variable": "#ffffff"
    }
  },
  
  // extensions
  "csharp.referencesCodeLens.enabled": false,
  "command-runner.terminal.autoFocus": true,
  "command-runner.terminal.cwd": "${fileDirname}",
  "command-runner.terminal.name": "script",
  "command-runner.commands": {
    "C#": "clear \ndotnet run",
    "C": "clear \nclang ${fileBasename} -o ${fileBasenameNoExtension} ; ./${fileBasenameNoExtension}.exe",
    "C++": "clear \nclang++ ${fileBasename} -o ${fileBasenameNoExtension} ; ./${fileBasenameNoExtension}.exe",
    "Python": "clear \npypy ${fileBasename}",
    "Java": "clear \njavac ${fileBasename} ; java ${fileBasenameNoExtension}",
    "Shell": "clear \nbash ${fileBasename}",
    "MGCB": "clear \nnmgcb-editor ${fileBasename}",
  },
  "errorLens.delay": 1,
  "errorLens.followCursor": "allLines",
  "errorLens.fontFamily": "Cascadia Code, monospace",
  "errorLens.gutterIconsEnabled": true,
  "errorLens.removeLinebreaks": false,
  "git.autofetch": true,
  "git.enableSmartCommit": true,
  "git.confirmSync": false,
  "todohighlight.isEnable": true,
  "todohighlight.isCaseSensitive": false,
  "todohighlight.maxFilesForSearch": 5120,
  "todohighlight.include": [
    "**/*.*",
  ],
  "todohighlight.keywords": [
    {
      "text": "TODO:",
      "color": "#ecf0f1",
      "border": "1px solid #e74c3c",
      "borderRadius": "4px",
      "backgroundColor": "#e74c3c",
    },
    {
      "text": "FIXME:",
      "color": "#ecf0f1",
      "border": "1px solid #f1c40f",
      "borderRadius": "4px",
      "backgroundColor": "#f1c40f",
    },
    {
      "text": "NOTE:",
      "color": "#ecf0f1",
      "border": "1px solid #3498db",
      "borderRadius": "4px",
      "backgroundColor": "#3498db",
    },
    {
      "text": "HACK:",
      "color": "#ecf0f1",
      "border": "1px solid #9b59b6",
      "borderRadius": "4px",
      "backgroundColor": "#9b59b6",
    },
    {
      "text": "BUG:",
      "color": "#ecf0f1",
      "border": "1px solid #2ecc71",
      "borderRadius": "4px",
      "backgroundColor": "#2ecc71",
    },
    {
      "text": "XXX:",
      "color": "#ecf0f1",
      "border": "1px solid #3c3d4d",
      "borderRadius": "4px",
      "backgroundColor": "#3c3d4d",
    },
  ],
}
~~~

### ⌨️ Keybindings
~~~json with comments
[
    {
      "key": "alt+oem_plus",
      "command": "editor.action.fontZoomIn"
    },
    {
      "key": "alt+oem_minus",
      "command": "editor.action.fontZoomOut"
    },
    {
      "key": "ctrl+alt+backspace",
      "command": "editor.action.fontZoomReset"
    },
    {
      "key": "shift+alt+t",
      "command": "todohighlight.listAnnotations"
    },
]
~~~
