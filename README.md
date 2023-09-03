<h1 align="center">
    My Visual Studio Code configuration
</h1>

> [!NOTE]
> This is my configuration for Visual Studio Code. The key bindings can be difficult to understand. You can see with the keybindings.json and the keybinding extentions.

> [!WARNING]
> I only added extensions that change Visual Studio Code or add features, not the ones related to programming languages.

## 🖼️ Screenshots
![](./screenshots/screenshot1.png)
![](./screenshots/screenshot2.png)

## 🗒️ Font
- [JetBrains Mono](https://github.com/JetBrains/JetBrainsMono)

## 🏞️ Theme
- [Yellowed Marketplace](https://marketplace.visualstudio.com/items?itemName=gael-lopes-da-silva.yellowed)
- [Yellowed Github](https://github.com/Gael-Lopes-Da-Silva/Yellowed)

## ⚙️ Extensions
- [Better Align](https://marketplace.visualstudio.com/items?itemName=Chouzz.vscode-better-align)
- [Choose a License](https://marketplace.visualstudio.com/items?itemName=ultram4rine.vscode-choosealicense)
- [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
- [CodeSnap](https://marketplace.visualstudio.com/items?itemName=adpyke.codesnap)
- [Command Runner](https://marketplace.visualstudio.com/items?itemName=edonet.vscode-command-runner)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [File System Toolbox](https://marketplace.visualstudio.com/items?itemName=CarloCardella.vscode-filesystemtoolbox)
- [File Utils](https://marketplace.visualstudio.com/items?itemName=sleistner.vscode-fileutils)
- [Font Preview](https://marketplace.visualstudio.com/items?itemName=AdamRaichu.font-viewer)
- [GitHub Repositories](https://marketplace.visualstudio.com/items?itemName=GitHub.remotehub)
- [Go To Method](https://marketplace.visualstudio.com/items?itemName=trixnz.go-to-method)
- [Hex Editor](https://marketplace.visualstudio.com/items?itemName=ms-vscode.hexeditor)
- [Increment Selection](https://marketplace.visualstudio.com/items?itemName=albymor.increment-selection)
- [IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)
- [IntelliCode Completions](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode-completions)
- [Jump](https://marketplace.visualstudio.com/items?itemName=wenfangdu.jump)
- [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)
- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
- [Markdown Emoji](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-emoji)
- [Mizu Icons](https://marketplace.visualstudio.com/items?itemName=cdfzo.mizu)
- [Output Colorizer](https://marketplace.visualstudio.com/items?itemName=IBM.output-colorizer)
- [Output Link to File](https://marketplace.visualstudio.com/items?itemName=93akkord.output-link-to-file)
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
- [Path Tools](https://marketplace.visualstudio.com/items?itemName=cg-cnu.vscode-path-tools)
- [Peek Hidden Files](https://marketplace.visualstudio.com/items?itemName=adrianwilczynski.toggle-hidden)
- [Perfect Line Selection](https://marketplace.visualstudio.com/items?itemName=erhise.perfect-line-selection)
- [QR Code Generator](https://marketplace.visualstudio.com/items?itemName=Compulim.vscode-qrcode)
- [Random Everthing](https://marketplace.visualstudio.com/items?itemName=helixquar.randomeverything)
- [Remote Repositories](https://marketplace.visualstudio.com/items?itemName=ms-vscode.remote-repositories)
- [Terminal All In One](https://marketplace.visualstudio.com/items?itemName=yasht.terminal-all-in-one)
- [Text Toolbox](https://marketplace.visualstudio.com/items?itemName=CarloCardella.vscode-texttoolbox)
- [TODO Highlight v2](https://marketplace.visualstudio.com/items?itemName=jgclark.vscode-todo-highlight)

## 🔧 Settings
~~~json with comments
{
    // sync
    "settingsSync.ignoredSettings": [
        "-C_Cpp.default.compilerPath",
        "terminal.external.windowsExec"
    ],

    // theme
    "editor.semanticHighlighting.enabled": false,
    "editor.semanticTokenColorCustomizations": {
        "enabled": false
    },

    // languages
    "C_Cpp.autoAddFileAssociations": false,
    "C_Cpp.autocomplete": "default",
    "C_Cpp.autocompleteAddParentheses": true,
    "C_Cpp.clang_format_sortIncludes": true,
    "C_Cpp.debugShortcut": false,
    "C_Cpp.default.compilerPath": "Your path",
    "C_Cpp.enhancedColorization": "disabled",
    "java.inlayHints.parameterNames.enabled": "none",
    "Lua.semantic.enable": false,
    "redhat.telemetry.enabled": false,

    // extensions
    "code-runner.clearPreviousOutput": true,
    "code-runner.enableAppInsights": false,
    "code-runner.executorMapByGlob": {
        "*.c": "clang $fullFileName -o $fileNameWithoutExt && $fileNameWithoutExt",
        "*.cpp": "clang++ $fullFileName -o $fileNameWithoutExt && $fileNameWithoutExt",
        "*.cs": "dotnet run --project $workspaceRoot",
        "*.java": "javac $fullFileName && java $fileNameWithoutExt",
        "*.nim": "nim compile --run --hints:off --spellSuggest:0 $fullFileName",
        "*.nims": "nim --run --hints:off --spellSuggest:0 $fullFileName",
        "*.py": "python $fullFileName",
        "*.sh": "sh $fullFileName"
    },
    "code-runner.fileDirectoryAsCwd": true,
    "code-runner.ignoreSelection": true,
    "code-runner.saveAllFilesBeforeRun": true,
    "code-runner.saveFileBeforeRun": true,
    "code-runner.showRunCommandInEditorContextMenu": false,
    "code-runner.showRunCommandInExplorerContextMenu": false,
    "code-runner.showRunIconInEditorTitleMenu": false,
    "code-runner.showStopIconInEditorTitleMenu": false,
    "codesnap.showLineNumbers": false,
    "codesnap.showWindowControls": false,
    "codesnap.transparentBackground": true,
    "command-runner.terminal.autoClear": false,
    "command-runner.terminal.autoFocus": true,
    "command-runner.terminal.cwd": "${fileDirname}",
    "command-runner.terminal.name": "script",
    "errorLens.borderRadius": "3px",
    "errorLens.delay": 100,
    "errorLens.enabled": true,
    "errorLens.enabledInMergeConflict": true,
    "errorLens.enableOnDiffView": true,
    "errorLens.followCursor": "allLines",
    "errorLens.fontSize": "14",
    "errorLens.messageBackgroundMode": "message",
    "errorLens.messageTemplate": "$message",
    "errorLens.onSave": false,
    "errorLens.padding": "0px 10px 0px 10px",
    "errorLens.removeLinebreaks": false,
    "errorLens.scrollbarHackEnabled": true,
    "hexeditor.columnWidth": 17,
    "hexeditor.defaultEndianness": "little",
    "hexeditor.inspectorType": "aside",
    "hexeditor.showDecodedText": true,
    "license.author": "Your name",
    "license.default": "bsd-3-clause",
    "license.extension": ".md",
    "license.year": "auto",
    "markdown.extension.list.indentationSize": "inherit",
    "markdown.extension.theming.decoration.renderCodeSpan": true,
    "terminalAllInOne.disableAllMessages": true,
    "terminalAllInOne.script.disableDescription": true,
    "terminalAllInOne.scripts": [],
    "todohighlight.isEnable": true,
    "todohighlight.isCaseSensitive": true,
    "todohighlight.include": ["**/*.*"],
    "todohighlight.defaultStyle": {
        "backgroundColor": "#00000000",
        "fontWeight": "bold",
        "isWholeLine": false
    },
    "todohighlight.keywords": [
        {
            "text": "TODO",
            "color": "#f1c40f",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)TODO(?!\\w)"
            }
        },
        {
            "text": "WARNING",
            "color": "#f1c40f",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)WARNING(?!\\w)"
            }
        },
        {
            "text": "XXX",
            "color": "#f1c40f",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)XXX(?!\\w)"
            }
        },
        {
            "text": "FIXME",
            "color": "#e74c3c",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)FIXME(?!\\w)"
            }
        },
        {
            "text": "FIX",
            "color": "#e74c3c",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)FIX(?!\\w)"
            }
        },
        {
            "text": "NOTE",
            "color": "#3498db",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)NOTE(?!\\w)"
            }
        },
        {
            "text": "HACK",
            "color": "#9b59b6",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)HACK(?!\\w)"
            }
        },
        {
            "text": "PERF",
            "color": "#9b59b6",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)PERF(?!\\w)"
            }
        },
        {
            "text": "PERFORMANCE",
            "color": "#9b59b6",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)PERFORMANCE(?!\\w)"
            }
        },
        {
            "text": "OPTIM",
            "color": "#9b59b6",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)OPTIM(?!\\w)"
            }
        },
        {
            "text": "OPTIMIZE",
            "color": "#9b59b6",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)OPTIMIZE(?!\\w)"
            }
        },
        {
            "text": "BUG",
            "color": "#2ecc71",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)BUG(?!\\w)"
            }
        },
        {
            "text": "TESTING",
            "color": "#00ffea",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)TESTING(?!\\w)"
            }
        },
        {
            "text": "PASSED",
            "color": "#00ff00",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)PASSED(?!\\w)"
            }
        },
        {
            "text": "FAILED",
            "color": "#ff0000",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)FAILED(?!\\w)"
            }
        },
    ],

    // settings
    "breadcrumbs.enabled": true,
    "breadcrumbs.filePath": "off",
    "breadcrumbs.icons": true,
    "debug.console.closeOnEnd": true,
    "debug.openDebug": "neverOpen",
    "debug.saveBeforeStart": "allEditorsInActiveGroup",
    "debug.terminal.clearBeforeReusing": true,
    "diffEditor.codeLens": true,
    "diffEditor.wordWrap": "inherit",
    "editor.autoClosingBrackets": "languageDefined",
    "editor.autoClosingQuotes": "languageDefined",
    "editor.autoIndent": "full",
    "editor.bracketPairColorization.enabled": false,
    "editor.codeLens": true,
    "editor.colorDecorators": true,
    "editor.cursorBlinking": "solid",
    "editor.cursorStyle": "block",
    "editor.cursorWidth": 3,
    "editor.definitionLinkOpensInPeek": false,
    "editor.detectIndentation": true,
    "editor.dragAndDrop": false,
    "editor.emptySelectionClipboard": true,
    "editor.fastScrollSensitivity": 5,
    "editor.find.seedSearchStringFromSelection": "selection",
    "editor.find.autoFindInSelection": "multiline",
    "editor.folding": false,
    "editor.foldingHighlight": false,
    "editor.foldingStrategy": "auto",
    "editor.fontFamily": "JetBrains Mono, Cascadia Code, Source Code Pro",
    "editor.fontLigatures": true,
    "editor.fontSize": 18,
    "editor.gotoLocation.multipleDefinitions": "goto",
    "editor.guides.bracketPairs": false,
    "editor.guides.indentation": true,
    "editor.hideCursorInOverviewRuler": false,
    "editor.inlayHints.enabled": "on",
    "editor.inlayHints.fontSize": 11,
    "editor.inlayHints.padding": true,
    "editor.inlineSuggest.enabled": true,
    "editor.inlineSuggest.showToolbar": "onHover",
    "editor.insertSpaces": true,
    "editor.largeFileOptimizations": true,
    "editor.letterSpacing": 0.2,
    "editor.lightbulb.enabled": false,
    "editor.lineHeight": 22,
    "editor.lineNumbers": "off",
    "editor.linkedEditing": false,
    "editor.links": true,
    "editor.matchBrackets": "always",
    "editor.minimap.enabled": false,
    "editor.overviewRulerBorder": false,
    "editor.padding.bottom": 20,
    "editor.padding.top": 20,
    "editor.quickSuggestionsDelay": 0,
    "editor.renderLineHighlight": "line",
    "editor.renderWhitespace": "none",
    "editor.scrollBeyondLastColumn": 4,
    "editor.scrollBeyondLastLine": false,
    "editor.showFoldingControls": "always",
    "editor.smoothScrolling": false,
    "editor.suggest.filterGraceful": true,
    "editor.suggest.insertMode": "replace",
    "editor.suggest.localityBonus": true,
    "editor.suggest.matchOnWordStartOnly": true,
    "editor.suggest.preview": true,
    "editor.suggest.selectionMode": "always",
    "editor.tabSize": 4,
    "editor.unicodeHighlight.ambiguousCharacters": true,
    "editor.unicodeHighlight.includeComments": false,
    "editor.unicodeHighlight.includeStrings": false,
    "editor.unicodeHighlight.invisibleCharacters": true,
    "editor.unicodeHighlight.nonBasicASCII": false,
    "editor.wordWrap": "bounded",
    "editor.wordWrapColumn": 150,
    "editor.wrappingIndent": "same",
    "editor.wrappingStrategy": "simple",
    "explorer.autoReveal": false,
    "explorer.compactFolders": false,
    "explorer.confirmDelete": false,
    "explorer.confirmDragAndDrop": false,
    "explorer.excludeGitIgnore": false,
    "explorer.incrementalNaming": "smart",
    "extensions.ignoreRecommendations": true,
    "files.autoSave": "afterDelay",
    "files.autoSaveDelay": 1000,
    "files.enableTrash": true,
    "files.encoding": "utf8",
    "files.eol": "\n",
    "files.exclude": {
        "**/.config": true,
        "**/.git": true,
        "**/.godot": true,
        "**/.vs": true,
        "**/bin": true,
        "**/obj": true,
    },
    "files.insertFinalNewline": false,
    "files.refactoring.autoSave": true,
    "files.restoreUndoStack": true,
    "files.saveConflictResolution": "overwriteFileOnDisk",
    "files.simpleDialog.enable": true,
    "git.autofetch": true,
    "git.closeDiffOnOperation": true,
    "git.confirmSync": false,
    "git.enableSmartCommit": true,
    "git.fetchOnPull": true,
    "git.useEditorAsCommitInput": true,
    "notebook.showFoldingControls": "always",
    "security.workspace.trust.enabled": false,
    "telemetry.telemetryLevel": "off",
    "terminal.external.windowsExec": "Your path",
    "terminal.integrated.customGlyphs": true,
    "terminal.integrated.enableFileLinks": "on",
    "terminal.integrated.gpuAcceleration": "on",
    "terminal.integrated.shellIntegration.enabled": true,
    "terminal.integrated.showLinkHover": true,
    "terminal.integrated.tabFocusMode": false,
    "window.confirmBeforeClose": "keyboardOnly",
    "window.dialogStyle": "custom",
    "window.enableMenuBarMnemonics": false,
    "window.experimental.windowControlsOverlay.enabled": true,
    "window.menuBarVisibility": "hidden",
    "window.title": "${rootName}",
    "window.titleBarStyle": "custom",
    "window.zoomLevel": 0.8,
    "workbench.activityBar.visible": false,
    "workbench.colorTheme": "Yellowed Reborn",
    "workbench.commandPalette.experimental.suggestCommands": true,
    "workbench.editor.enablePreview": false,
    "workbench.editor.showTabs": false,
    "workbench.editor.tabCloseButton": "off",
    "workbench.editor.tabSizing": "shrink",
    "workbench.iconTheme": "mizu",
    "workbench.layoutControl.enabled": false,
    "workbench.startupEditor": "none",
    "workbench.statusBar.visible": false,
    "haskell.manageHLS": "PATH",
}
~~~

## ⌨️ Keybindings
~~~json with comments
[
    // VSCode
    {
        "key": "shift shift",
        "command": "workbench.action.showCommands"
    },
    {
        "key": "ctrl+0 ctrl+0",
        "command": "editor.action.fontZoomReset"
    },
    {
        "key": "ctrl+=",
        "command": "editor.action.fontZoomIn"
    },
    {
        "key": "ctrl+-",
        "command": "editor.action.fontZoomOut"
    },

    // Keymap
    {
        "key": "alt+p",
        "command": "workbench.action.quickOpen"
    },
    {
        "key": "alt+o",
        "command": "workbench.action.files.openFile"
    },
    {
        "key": "alt+shift+o",
        "command": "workbench.action.files.openFolder"
    },
    {
        "key": "alt+b",
        "command": "workbench.action.toggleSidebarVisibility"
    },
    {
        "key": "alt+s",
        "command": "editor.action.addSelectionToNextFindMatch",
        "when": "textInputFocus"
    },
    {
        "key": "alt+x",
        "command": "extension.selectPerfectLine",
        "when": "textInputFocus"
    },
    {
        "key": "alt+f",
        "command": "editor.action.showDefinitionPreviewHover",
        "when": "textInputFocus"
    },
    {
        "key": "alt+v",
        "command": "expandLineSelection",
        "when": "textInputFocus"
    },
    {
        "key": "alt+n",
        "command": "workbench.action.terminal.toggleTerminal",
        "when": "terminal.active"
    },
    {
        "key": "alt+i",
        "command": "editor.action.insertSnippet",
        "when": "!editorReadonly && !editorReadonly"
    },
    {
        "key": "alt+/",
        "command": "editor.action.commentLine",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "alt+'",
        "command": "editor.action.triggerSuggest",
        "when": "editorHasCompletionItemProvider && textInputFocus && !editorReadonly"
    },
    {
        "key": "alt+'",
        "command": "toggleSuggestionDetails",
        "when": "suggestWidgetVisible && textInputFocus"
    },
    {
        "key": "alt+u",
        "command": "undo"
    },
    {
        "key": "alt+shift+u",
        "command": "redo"
    },
    {
        "key": "ctrl+j ctrl+e",
        "command": "workbench.view.explorer",
        "when": "viewContainer.workbench.view.explorer.enabled"
    },
    {
        "key": "ctrl+j ctrl+g",
        "command": "workbench.view.scm",
        "when": "workbench.scm.active"
    },
    {
        "key": "ctrl+j ctrl+b",
        "command": "workbench.action.toggleActivityBarVisibility"
    },
    {
        "key": "ctrl+j ctrl+z",
        "command": "workbench.action.toggleZenMode"
    },
    {
        "key": "alt+g alt+l",
        "command": "cursorEnd",
        "when": "textInputFocus"
    },
    {
        "key": "alt+g alt+h",
        "command": "cursorHome",
        "when": "textInputFocus"
    },
    {
        "key": "alt+g alt+k",
        "command": "cursorTop",
        "when": "textInputFocus"
    },
    {
        "key": "alt+g alt+j",
        "command": "cursorBottom",
        "when": "textInputFocus"
    },
    {
        "key": "alt+g alt+g",
        "command": "workbench.action.gotoLine"
    },
    {
        "key": "alt+j",
        "command": "cursorDown",
        "when": "textInputFocus"
    },
    {
        "key": "alt+k",
        "command": "cursorUp",
        "when": "textInputFocus"
    },
    {
        "key": "alt+h",
        "command": "cursorLeft",
        "when": "textInputFocus"
    },
    {
        "key": "alt+l",
        "command": "cursorRight",
        "when": "textInputFocus"
    },
    {
        "key": "alt+shift+j",
        "command": "cursorDownSelect",
        "when": "textInputFocus"
    },
    {
        "key": "alt+shift+k",
        "command": "cursorUpSelect",
        "when": "textInputFocus"
    },
    {
        "key": "alt+shift+h",
        "command": "cursorLeftSelect",
        "when": "textInputFocus"
    },
    {
        "key": "alt+shift+l",
        "command": "cursorRightSelect",
        "when": "textInputFocus"
    },
    {
        "key": "alt+ctrl+h",
        "command": "cursorWordLeft",
        "when": "textInputFocus"
    },
    {
        "key": "alt+ctrl+l",
        "command": "cursorWordRight",
        "when": "textInputFocus"
    },
    {
        "key": "alt+shift+ctrl+h",
        "command": "cursorWordLeftSelect",
        "when": "textInputFocus"
    },
    {
        "key": "alt+shift+ctrl+l",
        "command": "cursorWordRightSelect",
        "when": "textInputFocus"
    },
    {
        "key": "alt+j",
        "command": "workbench.action.quickOpenSelectNext",
        "when": "inQuickOpen"
    },
    {
        "key": "alt+k",
        "command": "workbench.action.quickOpenSelectPrevious",
        "when": "inQuickOpen"
    },
    {
        "key": "alt+j",
        "command": "selectNextSuggestion",
        "when": "suggestWidgetMultipleSuggestions && suggestWidgetVisible && textInputFocus"
    },
    {
        "key": "alt+k",
        "command": "selectPrevSuggestion",
        "when": "suggestWidgetMultipleSuggestions && suggestWidgetVisible && textInputFocus"
    },
    {
        "key": "alt+enter",
        "command": "editor.action.insertLineAfter",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "alt+shift+enter",
        "command": "editor.action.insertLineBefore",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "alt+backspace",
        "command": "editor.action.deleteLines",
        "when": "editorTextFocus"
    },
    {
        "key": "alt+c",
        "command": "editor.action.insertCursorBelow",
        "when": "editorTextFocus"
    },
    {
        "key": "alt+shift+c",
        "command": "editor.action.insertCursorAbove",
        "when": "editorTextFocus"
    },
]
~~~
