<h3 align="center">Visual Studio Code configuration</h3>

---

<p align="center">⚙️ This is my configuration for Visual Studio Code. The key bindings can be difficult to understand. You can see with the keybindings.json and the keybinding extention.</p>

<p align="center">⚠️ I only added the extensions that change vs code, not the ones related to the languages.</p>

---

### 🖼️ Screenshots
![](https://cdn.discordapp.com/attachments/594977170850447411/1002193478329061428/Capture_decran_2022-07-28_143318.png)
![](https://cdn.discordapp.com/attachments/594977170850447411/1002193478719127633/Capture_decran_2022-07-28_143446.png)
![](https://cdn.discordapp.com/attachments/594977170850447411/1002193479138545734/Capture_decran_2022-07-28_143710.png)

### 📃 Font
- [Cascadia Mono](https://github.com/microsoft/cascadia-code)

### 🏞️ Theme
- [Yellowed Marketplace](https://marketplace.visualstudio.com/items?itemName=gael-lopes-da-silva.yellowed)
- [Yellowed Github](https://github.com/Gael-Lopes-Da-Silva/Yellowed)

### ⚙️ Extensions
- [Better Align](https://marketplace.visualstudio.com/items?itemName=wwm.better-align)
- [Choose a License](https://marketplace.visualstudio.com/items?itemName=ultram4rine.vscode-choosealicense)
- [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
- [Command Runner](https://marketplace.visualstudio.com/items?itemName=edonet.vscode-command-runner)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [Hex Editor](https://marketplace.visualstudio.com/items?itemName=ms-vscode.hexeditor)
- [IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)
- [IntelliCode Completions](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode-completions)
- [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)
- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
- [Material Product Icons](https://marketplace.visualstudio.com/items?itemName=PKief.material-product-icons)
- [NERDTree](https://marketplace.visualstudio.com/items?itemName=Llam4u.nerdtree)
- [Output Colorizer](https://marketplace.visualstudio.com/items?itemName=IBM.output-colorizer)
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
- [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)
- [Vimspired](https://marketplace.visualstudio.com/items?itemName=bmalehorn.vimspired)

### 🔧 Settings
~~~json with comments
{
    // keybindings
    "vimspired.keybindings": {
        "i": "vimspired.toggle",

        "k": "cursorUp",
        "j": "cursorDown",
        "h": "cursorLeft",
        "l": "cursorRight",
        "K": "cursorUpSelect",
        "J": "cursorDownSelect",
        "H": "cursorLeftSelect",
        "L": "cursorRightSelect",

        ">": {"selecting": "cursorTopSelect", "default": "cursorTop"},
        "<": {"selecting": "cursorBottomSelect", "default": "cursorBottom"},
        ".": {"selecting": "cursorEndSelect", "default": "cursorEnd"},
        ",": {"selecting": "cursorHomeSelect", "default": "cursorHome"},

        "/": "actions.find",
        ";": "editor.action.triggerSuggest",
        "c": ["editor.action.clipboardCopyAction", "vimspired.cancelSelection"],
        "p": "editor.action.clipboardPasteAction",
        "u": "undo",
        "r": "redo",
        "[": "editor.fold",
        "]": "editor.unfold",

        "o": ["editor.action.insertLineAfter", "vimspired.enterInsert"],
        "O": ["editor.action.insertLineBefore", "vimspired.enterInsert"],

        "v": { // viewport
            ".": {"command": "editorScroll", "args": {"to": "up", "by": "halfPage"}},
            ",": {"command": "editorScroll", "args": {"to": "down", "by": "halfPage"}},
            "<": {"command": "editorScroll", "args": {"to": "down", "by": "page"}},
            ">": {"command": "editorScroll", "args": {"to": "up", "by": "page"}},
        },

        "m": { // move
            "j": {"command": "cursorMove", "args": {"to": "prevBlankLine"}},
            "k": {"command": "cursorMove", "args": {"to": "nextBlankLine"}},
            "c": {"command": "cursorMove", "args": {"to": "viewPortCenter"}},
            ">": {"command": "cursorMove", "args": {"to": "viewPortTop"}}, 
            "<": {"command": "cursorMove", "args": {"to": "viewPortBottom"}},
        },

        "w": { // word
            "d": "editor.action.goToDeclaration",          // declaration
            "r": "editor.action.rename",                   // rename
            "R": "editor.action.startFindReplaceAction",   // replace
            "f": "references-view.find",                   // reference
            "l": "editor.action.openLink",                 // link
            "a": "wwm.aligncode",                          // align
            "c": "editor.action.clipboardCutAction",       // cut
            "h": "editor.action.showHover",                // hover
            "p": "editor.action.triggerParameterHints",    // parameters
            "s": "editor.action.sortLinesAscending",       // sort
        },

        "s": { // select
            "a": "editor.action.selectAll",          // all
            "b": "editor.action.selectToBracket",    // brackets
            "o": "editor.action.selectHighlights",   // occurence
            "c": "vimspired.cancelSelection",        // cancel
        },

        "S": { // sidebar
            "e": "workbench.view.explorer",                    // explorer
            "g": "workbench.view.scm",                         // git
            "d": "workbench.view.debug",                       // debuger
            "x": "workbench.view.extensions",                  // extensions
            "s": "workbench.action.findInFiles",               // search
            "r": "workbench.action.replaceInFiles",            // replace
            " ": "workbench.action.toggleSidebarVisibility",   // toggle
        },

        "a": { // anchor
            "a": "editor.action.setSelectionAnchor",         // add
            "s": "editor.action.selectFromAnchorToCursor",   // select
            "j": "editor.action.goToSelectionAnchor",        // jump
            "c": "editor.action.cancelSelectionAnchor",      // cancel
        },

        "d": { // delete
            "s": "deleteLeft",                           // selection
            "l": "editor.action.deleteLines",            // line
            "w": "deleteInsideWord",                     // word
            "d": "editor.action.removeDuplicateLines",   // duplicates
            "L": "deleteAllLeft",                        // left
            "R": "deleteAllRight",                       // right
        },

        " ": { // leader
            "F": { // folder
                "o": "workbench.action.files.openFolder",   // open
                "c": "workbench.action.closeFolder",        // close
                "n": "explorer.newFolder",                  // new
            },
            "f": { // file
                "o": "workbench.action.files.openFile",              // open
                "c": "workbench.action.closeActiveEditor",           // close
                "s": "workbench.action.files.save",                  // save
                "S": "workbench.action.files.saveFiles",             // save all
                "g": "workbench.action.gotoLine",                    // go to
                "l": "workbench.action.editor.changeLanguageMode",   // language
                "f": "editor.action.formatDocument",                 // format
                "r": "editor.action.rename",                         // rename
                "p": "copyFilePath",                                 // path
                "P": "copyRelativeFilePath",                         // relative path
                "n": "explorer.newFile",                             // new
            },
            "c": { // commands
                "r": "command-runner.run",              // run
                "p": "workbench.action.showCommands",   // palette
                "d": "workbench.action.debug.start",    // debug
            },
            "g": { // git
                "c": "git.commit",   // commit
                "p": "git.push",     // push
                "P": "git.pull",     // pull
                "C": "git.clone",    // clone
                "i": "git.init",     // init
            },
            "o": { // options
                "s": "workbench.action.openSettingsJson",            // settings
                "k": "workbench.action.openGlobalKeybindingsFile",   // keysettings
                "r": "workbench.action.reloadWindow",                // reload
                "S": "workbench.action.openGlobalKeybindings",       // shortcuts
                "w": "editor.action.toggleRenderWhitespace",         // whitespace
            }
        }
    },

    // extensions
    "vimspired.insertCursorStyle": "line",
    "vimspired.normalCursorStyle": "block",
    "material-icon-theme.hidesExplorerArrows": true,
    "liveServer.settings.donotShowInfoMsg": true,
    "C_Cpp.autocomplete": "Default",
    "C_Cpp.autocompleteAddParentheses": true,
    "C_Cpp.debugShortcut": false,
    "C_Cpp.autoAddFileAssociations": true,
    "C_Cpp.default.compilerPath": "C:\\Users\\Oasis\\Applications\\Clang\\bin\\gcc.exe",
    "license.author": "Gael Lopes Da Silva",
    "license.extension": ".md",
    "license.year": "auto",
    "license.default": "MIT",
    "csharp.suppressBuildAssetsNotification": true,
    "omnisharp.enableImportCompletion": true,
    "omnisharp.organizeImportsOnFormat": true,
    "omnisharp.autoStart": true,
    "code-runner.clearPreviousOutput": true,
    "code-runner.enableAppInsights": false,
    "code-runner.ignoreSelection": true,
    "code-runner.saveAllFilesBeforeRun": true,
    "code-runner.saveFileBeforeRun": true,
    "code-runner.showRunCommandInEditorContextMenu": false,
    "code-runner.showRunCommandInExplorerContextMenu": false,
    "code-runner.showRunIconInEditorTitleMenu": false,
    "code-runner.showStopIconInEditorTitleMenu": false,
    "code-runner.fileDirectoryAsCwd": true,
    "code-runner.executorMapByGlob": {
        "*.c"     : "cc $fullFileName -o $fileNameWithoutExt && ./$fileNameWithoutExt",
        "*.cs"    : "dotnet run $dir",
        "*.go"    : "go run .",
        "*.py"    : "python $fullFileName",
        "*.nim"   : "nim compile --run --hints:off --spellSuggest:0 $fullFileName",
        "*.nims"  : "nim --run --hints:off --spellSuggest:0 $fullFileName",
        "*.java"  : "javac $fullFileName && java $fileNameWithoutExt",
        "*.sh"    : "sh $fullFileName",
        "*.ts"    : "deno run $fullFileName",
        "makefile": "make $fullFileName"
    },
    "command-runner.terminal.autoFocus": true,
    "command-runner.terminal.autoClear": false, 
    "command-runner.terminal.cwd": "${fileDirname}",
    "command-runner.terminal.name": "script",
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
                "pattern": "(?<=^|\"|:|\\s)TODO(?!\\w)"
            }
        },
        {
            "text"           : "FIXME",
            "color"          : "#e74c3c",
            "fontWeight"     : "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)FIXME(?!\\w)"
            }
        },
        {
            "text"           : "NOTE",
            "color"          : "#3498db",
            "fontWeight"     : "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)NOTE(?!\\w)"
            }
        },
        {
            "text"           : "HACK",
            "color"          : "#9b59b6",
            "fontWeight"     : "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)HACK(?!\\w)"
            }
        },
        {
            "text"           : "BUG",
            "color"          : "#2ecc71",
            "fontWeight"     : "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)BUG(?!\\w)"
            }
        }
    ],
    
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
    "editor.fontFamily": "Cascadia Mono, monospace",
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
    "editor.renderWhitespace": "none",
    "editor.renderLineHighlight": "all",
    "editor.suggestFontSize": 18,
    "editor.suggestLineHeight": 24,
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
    "explorer.excludeGitIgnore": false,
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
    "terminal.integrated.defaultProfile.windows": "Git Bash",
    "terminal.integrated.shellIntegration.enabled": true,
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
}
~~~

### ⌨️ Keybindings
~~~json with comments
[
    // vscode
    {
        "key": "alt+=",
        "command": "editor.action.fontZoomIn",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "alt+-",
        "command": "editor.action.fontZoomOut",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "shift+alt+backspace",
        "command": "editor.action.fontZoomReset",
        "when": "editorTextFocus && !editorReadonly"
    },
    // code runner
    {
        "key": "f5",
        "command": "code-runner.run",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "alt+f5",
        "command": "code-runner.stop",
        "when": "editorTextFocus && !editorReadonly"
    },

    // Vimspired
    {
        "key": "ctrl+;",
        "command": "editor.action.commentLine",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "alt+;",
        "command": "editor.action.blockComment",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "escape",
        "command": "hideSuggestWidget",
        "when": "suggestWidgetVisible && editorTextFocus && !editorReadonly"
    },
    {
        "key": "escape",
        "command": "removeSecondaryCursors",
        "when": "editorHasMultipleSelections && textInputFocus"
    },
    {
        "key": "escape",
        "command": "leaveSnippet",
        "when": "editorTextFocus && inSnippetMode"
    },
    {
        "key": "escape",
        "command": "closeParameterHints",
        "when": "editorFocus && parameterHintsVisible"
    },
    {
        "key": "ctrl+up",
        "command": "cursorMove",
        "args": {
            "to": "prevBlankLine"
        }
    },
    {
        "key": "ctrl+down",
        "command": "cursorMove",
        "args": {
            "to": "nextBlankLine"
        }
    },
    {
        "key": "ctrl+j",
        "command": "cursorMove",
        "when": "vimspired.normal",
        "args": {
            "to": "nextBlankLine"
        }
    },
    {
        "key": "ctrl+k",
        "command": "cursorMove",
        "when": "vimspired.normal",
        "args": {
            "to": "prevBlankLine"
        }
    },
    {
        "key": "ctrl+h",
        "command": "cursorWordLeft",
        "when": "vimspired.normal"
    },
    {
        "key": "ctrl+l",
        "command": "cursorWordRight",
        "when": "vimspired.normal"
    },
    {
        "key": "ctrl+alt+j",
        "command": "editor.action.insertCursorBelow",
        "when": "vimspired.normal"
    },
    {
        "key": "ctrl+alt+k",
        "command": "editor.action.insertCursorAbove",
        "when": "vimspired.normal"
    },
    {
        "key": "alt+j",
        "command": "editor.action.moveLinesDownAction",
        "when": "vimspired.normal"
    },
    {
        "key": "alt+k",
        "command": "editor.action.moveLinesUpAction",
        "when": "vimspired.normal"
    },
    {
        "key": "ctrl+shift+h",
        "command": "cursorWordLeftSelect",
        "when": "vimspired.normal"
    },
    {
        "key": "ctrl+shift+l",
        "command": "cursorWordEndRightSelect",
        "when": "vimspired.normal"
    }
]
~~~
