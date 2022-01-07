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
- [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
- [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
- [C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp)
- [Choose A License](https://marketplace.visualstudio.com/items?itemName=ultram4rine.vscode-choosealicense)
- [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
- [Monokai Accents](https://marketplace.visualstudio.com/items?itemName=tw.monokai-accent)
- [Nim](https://marketplace.visualstudio.com/items?itemName=nimsaem.nimvscode)
- [NuGet Package Manager GUI](https://marketplace.visualstudio.com/items?itemName=aliasadidev.nugetpackagemanagergui)
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [Visual Studio IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)

### 🔧 Settings
~~~json with comments
{
  // options
  "editor.suggestSelection": "first",
  "editor.suggest.preview": true,
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
  "editor.lineHeight": 20,
  "editor.fontSize": 17,
  "editor.fontFamily": "Cascadia Code, monospace",
  "editor.codeLensFontFamily": "Cascadia Code, monospace",
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
  "terminal.integrated.fontFamily": "CaskaydiaCove Nerd Font Mono, monospace",
  "terminal.integrated.customGlyphs": true,
  "terminal.integrated.gpuAcceleration": "auto",
  
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
          "entity.other.attribute-name.pseudo-class.css"
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
  
  // synchronization
  "settingsSync.ignoredSettings": [
    "-window.zoomLevel"
  ],
  
  // extensions
  "csharp.referencesCodeLens.enabled": false,
  "C_Cpp.autoAddFileAssociations": false,
  "notebook.lineNumbers": "on",
  "errorLens.delay": 1,
  "errorLens.followCursor": "allLines",
  "errorLens.fontFamily": "Cascadia Code, monospace",
  "errorLens.gutterIconsEnabled": true,
  "errorLens.removeLinebreaks": false,
  "errorLens.enabledDiagnosticLevels": [
    "error",
    "info"
  ],
  "git.autofetch": true,
  "git.enableSmartCommit": true,
  "git.confirmSync": false,
  "license.author": "Gaël Lopes Da Silva",
  "license.year": "auto",
  "code-runner.runInTerminal": true,
  "code-runner.saveFileBeforeRun": true,
  "code-runner.fileDirectoryAsCwd": true,
  "code-runner.ignoreSelection": true,
  "code-runner.executorMapByGlob": {
    "*.nims": "clear \nnim --run --verbosity:0 --spellSuggest:0 --hints:off $fileName",
    "*.nim": "clear \nnim compile --run --verbosity:0 --spellSuggest:0 --hints:off $fileName",
    "*.py": "clear \npypy $fileName",
    "*.sh": "clear \nbash $fileName",
    "*.c": "clear \nclang $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
    "*.cpp": "clear \nclang++ $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
    "*.java": "clear \njavac $fileName && java $fileNameWithoutExt",
    "*.cs": "clear \ndotnet run $fileName",
    "*.rs": "clear \nrustc $fileName && $dir$fileNameWithoutExt",
    "*.mgcb": "clear \nmgcb-editor $fileName",
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
  
  "window.zoomLevel": 1,
}
~~~

### ⌨️ Keybindings
~~~json with comments
[
    {
        "key": "ctrl+shift+r",
        "command": "code-runner.run"
    },
    {
        "key": "ctrl+shift+t",
        "command": "code-runner.stop"
    },
]
~~~
