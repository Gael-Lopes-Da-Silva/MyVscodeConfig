<h3 align="center">Visual Studio Code configuration</h3>

---

<p align="center">⚙️ This is my configuration for Visual Studio Code. The key bindings can be difficult to understand. You can see with the keybindings.json and the awesome emacs keymap extension.</p>

<p align="center">⚠️ I only added the extensions that change vs code, not the ones related to the languages.</p>

---

### 🖼️ Screenshots
![](https://cdn.discordapp.com/attachments/594977170850447411/980089463218778112/screenshot1.png)
![](https://cdn.discordapp.com/attachments/594977170850447411/980089463499784192/screenshot2.png)
![](https://cdn.discordapp.com/attachments/594977170850447411/980089462954541098/screenshot3.png)

### 📃 Font
- [JetBrains Mono](https://github.com/JetBrains/JetBrainsMono)

### 🏞️ Theme
- [Yellowed](https://marketplace.visualstudio.com/items?itemName=gael-lopes-da-silva.yellowed)

### ⚙️ Extensions
- [Awesome Emacs Keymap](https://marketplace.visualstudio.com/items?itemName=tuttieee.emacs-mcx)
- [Better Align](https://marketplace.visualstudio.com/items?itemName=wwm.better-align)
- [Choose a License](https://marketplace.visualstudio.com/items?itemName=ultram4rine.vscode-choosealicense)
- [Command Runner](https://marketplace.visualstudio.com/items?itemName=edonet.vscode-command-runner)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [Hex Editor](https://marketplace.visualstudio.com/items?itemName=ms-vscode.hexeditor)
- [IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)
- [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)
- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
- [Material Product Icons](https://marketplace.visualstudio.com/items?itemName=PKief.material-product-icons)
- [Output Colorizer](https://marketplace.visualstudio.com/items?itemName=IBM.output-colorizer)
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
- [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)

### 🔧 Settings
~~~json with comments
{
    // options
    "breadcrumbs.enabled": true,
    "breadcrumbs.filePath": "off",
    "breadcrumbs.icons": true,
    "debug.openDebug": "neverOpen",
    "debug.terminal.clearBeforeReusing": true,
    "diffEditor.codeLens": true,
    "diffEditor.wordWrap": "inherit",
    "editor.autoIndent": "full",
    "editor.autoClosingBrackets": "always",
    "editor.autoClosingQuotes": "always",
    "editor.bracketPairColorization.enabled": false,
    "editor.codeLens": true,
    "editor.colorDecorators": true,
    "editor.cursorWidth": 3,
    "editor.cursorStyle": "block",
    "editor.cursorBlinking": "solid",
    "editor.detectIndentation": false,
    "editor.dragAndDrop": false,
    "editor.emptySelectionClipboard": true,
    "editor.fastScrollSensitivity": 5,
    "editor.find.seedSearchStringFromSelection": "selection",
    "editor.folding": true,
    "editor.foldingHighlight": false,
    "editor.foldingStrategy": "auto",
    "editor.fontFamily": "JetBrains Mono, monospace",
    "editor.fontLigatures": false,
    "editor.fontSize": 18,
    "editor.fontWeight": "600",
    "editor.guides.indentation": true,
    "editor.guides.bracketPairs": false,
    "editor.hideCursorInOverviewRuler": false,
    "editor.insertSpaces": true,
    "editor.linkedEditing": false,
    "editor.largeFileOptimizations": true,
    "editor.letterSpacing": -0.3,
    "editor.lightbulb.enabled": false,
    "editor.links": true,
    "editor.lineHeight": 24,
    "editor.lineNumbers": "relative",
    "editor.matchBrackets": "always",
    "editor.minimap.enabled": false,
    "editor.overviewRulerBorder": false,
    "editor.padding.bottom": 1,
    "editor.padding.top": 1,
    "editor.quickSuggestionsDelay": 0,
    "editor.renderWhitespace": "selection",
    "editor.renderLineHighlight": "all",
    "editor.suggestFontSize": 18,
    "editor.suggestLineHeight": 24,
    "editor.suggestSelection": "first",
    "editor.suggest.preview": true,
    "editor.suggest.insertMode": "replace",
    "editor.tabSize": 4,
    "editor.unicodeHighlight.invisibleCharacters": false,
    "editor.wordWrap": "bounded",
    "editor.wordWrapColumn": 150,
    "editor.wrappingIndent": "same",
    "editor.wrappingStrategy": "simple",
    "explorer.compactFolders": true,
    "explorer.confirmDelete": false,
    "explorer.confirmDragAndDrop": false,
    "explorer.excludeGitIgnore": true,
    "explorer.incrementalNaming": "smart",
    "extensions.ignoreRecommendations": true,
    "files.autoSave": "afterDelay",
    "files.defaultLanguage": "${activeEditorLanguage}",
    "files.enableTrash": true,
    "files.encoding": "utf8",
    "files.eol": "\n",
    "files.insertFinalNewline": true,
    "files.restoreUndoStack": true,
    "files.saveConflictResolution": "overwriteFileOnDisk",
    "files.simpleDialog.enable": true,
    "git.autofetch": true,
    "git.confirmSync": false,
    "git.enableSmartCommit": true,
    "git.useEditorAsCommitInput": true,
    "security.workspace.trust.enabled": false,
    "terminal.integrated.customGlyphs": true,
    "terminal.integrated.enableFileLinks": true,
    "terminal.integrated.gpuAcceleration": "on",
    "terminal.integrated.showLinkHover": true,
    "window.dialogStyle": "custom",
    "window.menuBarVisibility": "hidden",
    "window.titleBarStyle": "custom",
    "window.title": "${rootName}${separator}${dirty}${activeEditorShort}${separator}${appName}",
    "window.confirmBeforeClose": "keyboardOnly",
    "window.enableMenuBarMnemonics": false,
    "window.experimental.windowControlsOverlay.enabled": true,
    "window.zoomLevel": 1,
    "workbench.activityBar.visible": false,
    "workbench.editor.enablePreview": false,
    "workbench.iconTheme": "material-icon-theme",
    "workbench.productIconTheme": "material-product-icons",
    "workbench.colorTheme": "Yellowed",

    // extensions
    "C_Cpp.autocompleteAddParentheses": true,
    "C_Cpp.debugShortcut": false,
    "material-icon-theme.hidesExplorerArrows": true,
    "redhat.telemetry.enabled": false,
    "license.author": "Gael Lopes Da Silva",
    "license.extension": "",
    "license.year": "auto",
    "license.default": "MIT",
    "csharp.referencesCodeLens.enabled": false,
    "csharp.suppressBuildAssetsNotification": true,
    "omnisharp.enableImportCompletion": true,
    "omnisharp.organizeImportsOnFormat": true,
    "omnisharp.useModernNet": false,
    "command-runner.terminal.autoFocus": true,
    "command-runner.terminal.autoClear": false, 
    "command-runner.terminal.cwd": "${fileDirname}",
    "command-runner.terminal.name": "script",
    "command-runner.commands": {
        // not simple
        "C"   : "clang -Wall -Wextra -pedantic -fno-common -fno-builtin ${file} -o ${fileBasenameNoExtension}.exe ; if ($?) {./${fileBasenameNoExtension}}",
        "C++" : "clang++ -Wall -Wextra -pedantic -fno-common -fno-builtin ${file} -o ${fileBasenameNoExtension}.exe ; if ($?) {./${fileBasenameNoExtension}}",
        "Java": "javac ${file} ; if ($?) {java ${fileBasenameNoExtension}}",

        // simple
        "Nim"      : "nim c -r --hints:off --spellSuggest:0 ${file}",
        "Nims"     : "nim -r --hints:off --spellSuggest:0 ${file}",
        "C#"       : "dotnet run",
        "C# Script": "dotnet script ${file}",
        "Go"       : "go run .",
        "Python"   : "python ${file}",
        "Batch"    : "powershell ${file}",
        "Shell"    : "sh ${file}",
        "Make"     : "make ${file}"
    },
    "markdown.extension.list.indentationSize": "inherit",
    "markdown.extension.syntax.decorations": true,
    "hexeditor.columnWidth": 16,
    "hexeditor.showDecodedText": true,
    "hexeditor.defaultEndianness": "little",
    "hexeditor.inspectorType": "aside",
    "errorLens.enabled": true,
    "errorLens.followCursor": "allLines",
    "errorLens.gutterIconsEnabled": true,
    "errorLens.messageBackgroundMode": "none",
    "errorLens.messageTemplate": "$severity: $message",
    "errorLens.removeLinebreaks": false,
    "errorLens.scrollbarHackEnabled": true,
    "todohighlight.isEnable": true,
    "todohighlight.isCaseSensitive": true,
    "todohighlight.include": ["**/*.*"],
    "todohighlight.exclude": [
        "**/node_modules/**",
        "**/bower_components/**",
        "**/dist/**",
        "**/build/**",
        "**/.vscode/**",
        "**/.vscode-test/**",
        "**/.github/**",
        "**/_output/**",
        "**/*.min.*",
        "**/*.map",
        "**/.next/**"
    ],
    "todohighlight.keywords": [
        {
            "text"           : "TODO",
            "color"          : "#f1c40f",
            "fontWeight"     : "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|\\s)TODO(?!\\w)"
            }
        },
        {
            "text"           : "FIXME",
            "color"          : "#e74c3c",
            "fontWeight"     : "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|\\s)FIXME(?!\\w)"
            }
        },
        {
            "text"           : "NOTE",
            "color"          : "#3498db",
            "fontWeight"     : "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|\\s)NOTE(?!\\w)"
            }
        },
        {
            "text"           : "HACK",
            "color"          : "#9b59b6",
            "fontWeight"     : "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|\\s)HACK(?!\\w)"
            }
        },
        {
            "text"           : "BUG",
            "color"          : "#2ecc71",
            "fontWeight"     : "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|\\s)BUG(?!\\w)"
            }
        }
    ]
}
~~~

### ⌨️ Keybindings
~~~json with comments
[
    // vscode
    {
        "key": "alt+=",
        "command": "editor.action.fontZoomIn"
    },
    {
        "key": "alt+-",
        "command": "editor.action.fontZoomOut"
    },
    {
        "key": "shift+alt+backspace",
        "command": "editor.action.fontZoomReset"
    },

    // todo highlight
    {
        "key": "ctrl+x t",
        "command": "todohighlight.listAnnotations"
    },

    // command runner
    {
        "key": "ctrl+x c",
        "command": "command-runner.run"
    },

    // error lens
    {
        "key": "ctrl+x e",
        "command": "errorLens.toggle"
    },

    // emacs
    {
        "key": "shift+space",
        "command": "editor.action.triggerSuggest",
        "when": "editorHasCompletionItemProvider && textInputFocus && !editorReadonly"
    },
    {
        "key": "ctrl+x ctrl+j",
        "command": "workbench.action.terminal.kill"
    },
    {
        "key": "ctrl+x j",
        "command": "workbench.action.terminal.new",
        "when": "terminalProcessSupported || terminalWebExtensionContributedProfile"
    },
    {
        "key": "ctrl+y",
        "command": "editor.action.clipboardPasteAction"
    },
    {
        "key": "ctrl+x /",
        "command": "redo"
    },
    {
        "key": "ctrl+x f",
        "command": "workbench.action.files.openFolder",
        "when": "openFolderWorkspaceSupport"
    },
    {
        "key": "ctrl+x l",
        "command": "workbench.action.editor.changeLanguageMode",
        "when": "!notebookEditorFocused && editorTextFocus"
    },
    {
        "key": "ctrl+up",
        "command": "emacs-mcx.backwardParagraph",
        "when": "editorTextFocus && !suggestWidgetVisible"
    },
    {
        "key": "ctrl+down",
        "command": "emacs-mcx.forwardParagraph",
        "when": "editorTextFocus && !suggestWidgetVisible"
    }
]
~~~
