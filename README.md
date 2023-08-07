<h3 align="center">
    Visual Studio Code configuration
</h3>

---

> [!NOTE]
> This is my configuration for Visual Studio Code. The key bindings can be difficult to understand. You can see with the keybindings.json and the keybinding extention.

> [!WARNING]
> I only added extensions that change Visual Studio Code or add features, not the ones related to programming languages.

---

### :framed_picture: Screenshots
![](https://github.com/Gael-Lopes-Da-Silva/Yellowed/blob/5486fccb6685e7339403db535a4e35b5025511e7/screenshots/screenshot1.png?raw=true)
![](https://github.com/Gael-Lopes-Da-Silva/Yellowed/blob/5486fccb6685e7339403db535a4e35b5025511e7/screenshots/screenshot2.png?raw=true)
![](https://github.com/Gael-Lopes-Da-Silva/Yellowed/blob/5486fccb6685e7339403db535a4e35b5025511e7/screenshots/screenshot3.png?raw=true)

### :spiral_notepad: Font
- [Cascadia Mono](https://github.com/microsoft/cascadia-code)

### :national_park: Theme
- [Yellowed Marketplace](https://marketplace.visualstudio.com/items?itemName=gael-lopes-da-silva.yellowed)
- [Yellowed Github](https://github.com/Gael-Lopes-Da-Silva/Yellowed)

### :gear: Extensions
- [Better Align](https://marketplace.visualstudio.com/items?itemName=Chouzz.vscode-better-align)
- [Choose a License](https://marketplace.visualstudio.com/items?itemName=ultram4rine.vscode-choosealicense)
- [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
- [Command Runner](https://marketplace.visualstudio.com/items?itemName=edonet.vscode-command-runner)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [File System Toolbox](https://marketplace.visualstudio.com/items?itemName=CarloCardella.vscode-filesystemtoolbox)
- [File Utils](https://marketplace.visualstudio.com/items?itemName=sleistner.vscode-fileutils)
- [GitHub Issue Notebooks](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-github-issue-notebooks)
- [GitHub Repositories](https://marketplace.visualstudio.com/items?itemName=GitHub.remotehub)
- [Go To Method](https://marketplace.visualstudio.com/items?itemName=trixnz.go-to-method)
- [Hex Editor](https://marketplace.visualstudio.com/items?itemName=ms-vscode.hexeditor)
- [Increment Selection](https://marketplace.visualstudio.com/items?itemName=albymor.increment-selection)
- [IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)
- [IntelliCode Completions](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode-completions)
- [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)
- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
- [Markdown Emoji](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-emoji)
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
- [Output Colorizer](https://marketplace.visualstudio.com/items?itemName=IBM.output-colorizer)
- [Output Link to File](https://marketplace.visualstudio.com/items?itemName=93akkord.output-link-to-file)
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
- [Path Tools](https://marketplace.visualstudio.com/items?itemName=cg-cnu.vscode-path-tools)
- [Peek Hidden Files](https://marketplace.visualstudio.com/items?itemName=adrianwilczynski.toggle-hidden)
- [Polacode](https://marketplace.visualstudio.com/items?itemName=pnp.polacode)
- [QR Code Generator](https://marketplace.visualstudio.com/items?itemName=Compulim.vscode-qrcode)
- [Random Everthing](https://marketplace.visualstudio.com/items?itemName=helixquar.randomeverything)
- [Remote Repositories](https://marketplace.visualstudio.com/items?itemName=ms-vscode.remote-repositories)
- [Svg Preview](https://marketplace.visualstudio.com/items?itemName=SimonSiefke.svg-preview)
- [Terminal All In One](https://marketplace.visualstudio.com/items?itemName=yasht.terminal-all-in-one)
- [Text Toolbox](https://marketplace.visualstudio.com/items?itemName=CarloCardella.vscode-texttoolbox)
- [TODO Highlight v2](https://marketplace.visualstudio.com/items?itemName=jgclark.vscode-todo-highlight)
- [Vimspired](https://marketplace.visualstudio.com/items?itemName=bmalehorn.vimspired)

### :wrench: Settings
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
        ">": "cursorTop",
        "<": "cursorBottom",
        ".": "cursorEnd",
        ",": "cursorHome",
        "/": "actions.find",
        ";": "editor.action.triggerSuggest",
        "c": [
            "editor.action.clipboardCopyAction",
            "vimspired.cancelSelection"
        ],
        "C": [
            "editor.action.selectAll",
            "editor.action.clipboardCopyAction",
            "vimspired.cancelSelection"
        ],
        "p": "editor.action.clipboardPasteAction",
        "u": "undo",
        "r": "redo",
        "[": "editor.fold",
        "]": "editor.unfold",
        "o": [
            "editor.action.insertLineAfter",
            "vimspired.enterInsert"
        ],
        "O": [
            "editor.action.insertLineBefore",
            "vimspired.enterInsert"
        ],
        "e": { // editor
            "l": "workbench.action.moveEditorRightInGroup", // right
            "h": "workbench.action.moveEditorLeftInGroup", // left
            "p": "workbench.action.pinEditor", // pin
            "u": "workbench.action.unpinEditor", // unpin
            "m": "workbench.action.showAllEditors", // menu
            "R": "workbench.action.reopenClosedEditor", // reopen
            "1": "workbench.action.previousEditor", // previous
            "2": "workbench.action.nextEditor", // next
        },
        "v": { // viewport
            ".": {
                "command": "editorScroll",
                "args": {
                    "to": "up",
                    "by": "halfPage"
                }
            },
            ",": {
                "command": "editorScroll",
                "args": {
                    "to": "down",
                    "by": "halfPage"
                }
            },
            "<": {
                "command": "editorScroll",
                "args": {
                    "to": "down",
                    "by": "page"
                }
            },
            ">": {
                "command": "editorScroll",
                "args": {
                    "to": "up",
                    "by": "page"
                }
            },
            "s": "editor.action.toggleStickyScroll", // sticky scroll
        },
        "m": { // move
            "j": {
                "command": "cursorMove",
                "args": {
                    "to": "nextBlankLine"
                }
            },
            "k": {
                "command": "cursorMove",
                "args": {
                    "to": "prevBlankLine"
                }
            },
            "c": {
                "command": "cursorMove",
                "args": {
                    "to": "viewPortCenter"
                }
            },
            ">": {
                "command": "cursorMove",
                "args": {
                    "to": "viewPortTop"
                }
            },
            "<": {
                "command": "cursorMove",
                "args": {
                    "to": "viewPortBottom"
                }
            },
            "l": "workbench.action.gotoLine", // line
            "b": "editor.action.jumpToBracket", // bracket
        },
        "w": { // word
            "r": "editor.action.rename", // rename
            "R": "editor.action.startFindReplaceAction", // replace
            "c": "editor.action.clipboardCutAction", // cut
            "l": "editor.action.openLink", // link
            "d": "editor.action.goToDeclaration", // declaration
            "h": "editor.action.showHover", // hover
            "p": "editor.action.triggerParameterHints", // parameters
            "a": "vscode-better-align.align", // align
            "s": { // sort
                "a": "editor.action.sortLinesAscending", // ascebing
                "d": "editor.action.sortLinesDescending", // descending
            },
        },
        "s": { // select
            "w": "editor.action.smartSelect.grow", // word
            "a": "editor.action.selectAll", // all
            "b": "editor.action.selectToBracket", // brackets
            "o": "editor.action.selectHighlights", // occurence
            "c": "vimspired.cancelSelection", // cancel
        },
        "a": { // anchor
            "a": "editor.action.setSelectionAnchor", // add
            "s": "editor.action.selectFromAnchorToCursor", // select
            "j": "editor.action.goToSelectionAnchor", // jump
            "c": "editor.action.cancelSelectionAnchor", // cancel
        },
        "b": { // bookmark
            "t": "bookmarks.toggle", // toggle
            "n": "bookmarks.jumpToNext", // next
            "p": "bookmarks.jumpToPrevious", // previous
            "l": "bookmarks.list", // list
            "L": "bookmarks.listFromAllFiles", // list all
            "c": "bookmarks.clearFromAllFiles", // clear
        },
        "d": { // delete
            "l": "editor.action.deleteLines", // line
            "w": "deleteInsideWord", // word
            "d": "editor.action.removeDuplicateLines", // duplicates
            "L": "deleteAllLeft", // left
            "R": "deleteAllRight", // right
        },
        "t": { // text
            "f": "vscode-texttoolbox.FilterLinesUsingRegExpOrString", // filter
            "S": "vscode-texttoolbox.SplitSelection", // split
            "t": "vscode-texttoolbox.TabOut", // tab out
            "T": "vscode-texttoolbox.ToggleTabOut", // tab out toggle
            "O": "vscode-texttoolbox.transformToOrderedList", // ordered list
            "a": { // align
                "t": "vscode-texttoolbox.AlignAsTable", // table
                "h": "vscode-texttoolbox.AlignAsTableWithHeaders", // header
                "s": "vscode-texttoolbox.AlignToSeparator", // separator
            },
            "c": { // conversion
                "p": "vscode-texttoolbox.PascalCase", // pascal case
                "c": "vscode-texttoolbox.CamelCase", // camel case
                "C": "vscode-texttoolbox.ConstantCase", // constant case
                "h": "vscode-texttoolbox.HeaderCase", // header case
                "d": "vscode-texttoolbox.DotCase", // dot case
                "k": "vscode-texttoolbox.KebabCase", // kebab case
                "S": "vscode-texttoolbox.SentenceCase", // sentence case
                "s": "vscode-texttoolbox.SnakeCase", // snake case
                "i": "vscode-texttoolbox.InvertCase", // invert case
                "H": "vscode-texttoolbox.ConvertDecimalToHexadecimal", // hexadecimal
                "D": "vscode-texttoolbox.ConvertHexadecimalToDecimal", // decimal
            },
            "j": { // json
                "f": "vscode-texttoolbox.FixJson", // format
                "w": "vscode-texttoolbox.EscapeWin32PathInJson", // win32
                "m": "vscode-texttoolbox.MinifyJson", // minify
                "s": "vscode-texttoolbox.StringifyJson", // stringify
            },
            "p": { // pad
                "l": "vscode-texttoolbox.PadSelectionLeft", // left
                "r": "vscode-texttoolbox.PadSelectionRight", // right
            },
            "P": { // path
                "p": "vscode-texttoolbox.TransformPathToPosix", // posix
                "w": "vscode-texttoolbox.TransformPathToWin32", // win32
            },
            "i": { // insert
                "g": "vscode-texttoolbox.InsertGUID", // guid
                "G": "vscode-texttoolbox.InsertGuidAllZeros", // guid zeros
                "d": "vscode-texttoolbox.InsertDate", // date
                "r": "vscode-texttoolbox.PickRandom", // random
                "l": "vscode-texttoolbox.InsertLoremIpsum", // lorem
                "L": "vscode-texttoolbox.InsertLineNumbers", // line number
                "n": "vscode-texttoolbox.InsertSequenceNumbers", // numbers sequece
                "c": "vscode-texttoolbox.InsertCurrency", // currency
                "q": "qrcode.generateFromSelected", // qr code
            },
            "r": { // remove
                "b": "vscode-texttoolbox.RemoveBrackets", // brackets
                "q": "vscode-texttoolbox.RemoveQuotes", // quotes
                "e": "vscode-texttoolbox.RemoveAllEmptyLines", // empty lines
                "c": "vscode-texttoolbox.RemoveControlCharacters", // control characters
                "d": "vscode-texttoolbox.RemoveDuplicateLines", // duplicates
                "r": "vscode-texttoolbox.RemoveRedundantEmptyLines", // redundant empty lines
            },
            "h": { // highlight
                "h": "vscode-texttoolbox.HighlightText", // highlight
                "c": "vscode-texttoolbox.HighlightTextWithColor", // color
                "a": { // all
                    "i": "vscode-texttoolbox.HighlightAllMatchesCaseInsensitive", // insensitive
                    "I": "vscode-texttoolbox.HighlightAllMatchesCaseInsensitiveWithColor", // insensitive color
                    "s": "vscode-texttoolbox.HighlightAllMatchesCaseSensitive", // sensitive
                    "S": "vscode-texttoolbox.HighlightAllMatchesCaseSensitiveWithColor", // sensitive color
                },
                "r": { // remove
                    "r": "vscode-texttoolbox.RemoveHighlight", // remove
                    "a": "vscode-texttoolbox.RemoveAllHighlights", // all
                },
                "R": { // regex
                    "R": "vscode-texttoolbox.HighlightWithRegExpWithColor", // regex color
                    "r": "vscode-texttoolbox.HighlightWithRegExp", // regex
                },
            },
            "C": { // cycle
                "b": "vscode-texttoolbox.CycleBrackets", // brackets
                "q": "vscode-texttoolbox.CycleQuotes", // quotes
            },
            "o": { // open
                "n": "vscode-texttoolbox.OpenSelectionInNewEditor", // new editor
                "u": "vscode-texttoolbox.OpenPathOrUrlUnderCursor", // under cursor
            },
            "e": { // encode
                "b": "vscode-texttoolbox.convertToBase64", // base64
                "h": "vscode-texttoolbox.toHTML", // html
                "u": "vscode-texttoolbox.encodeUri", // uri
            },
            "d": { // decode
                "b": "vscode-texttoolbox.convertFromBase64", // base64
                "h": "vscode-texttoolbox.fromHTML", // html
                "u": "vscode-texttoolbox.decodeUri", // uri
                "j": "vscode-texttoolbox.decodeJWTToken", // jwt
            },
        },
        " ": { // leader
            "F": { // folder
                "o": "workbench.action.files.openFolder", // open
                "O": "revealFileInOS", // open exeplorer
                "c": "workbench.action.closeFolder", // close
                "s": "extension.showFiles", // show
                "h": "extension.hideFiles", // hide
                "t": "extension.toggleFiles", // toggle
            },
            "f": { // file
                "o": "workbench.action.files.openFile", // open
                "c": "workbench.action.closeActiveEditor", // close
                "s": "workbench.action.files.save", // save
                "S": "workbench.action.files.saveFiles", // save all
                "l": "workbench.action.editor.changeLanguageMode", // language
                "f": "editor.action.formatDocument", // format
                "r": "editor.action.rename", // rename
                "p": "copyFilePath", // path
                "P": "copyRelativeFilePath", // relative path
            },
            "s": { // sidebar
                "e": "workbench.view.explorer", // explorer
                "g": "workbench.view.scm", // git
                "d": "workbench.view.debug", // debuger
                "x": "workbench.view.extensions", // extensions
                "b": "workbench.view.extension.bookmarks", // bookmarks
                "s": "workbench.action.findInFiles", // search
                "r": "workbench.action.replaceInFiles", // replace
                " ": "workbench.action.toggleSidebarVisibility", // toggle
            },
            "c": { // commands
                "p": "workbench.action.showCommands", // palette
                "d": "workbench.action.debug.start", // debug
                "c": "command-runner.run", // commands
                "r": "code-runner.run", // run
                "s": "code-runner.stop", // stop
            },
            "C": { // console
                "n": "workbench.action.terminal.new", // new
                "k": "workbench.action.terminal.kill", // kill
                "K": "workbench.action.terminal.killAll", // kill all
            },
            "g": { // git
                "C": "git.clone", // clone
                "D": "git.cleanAll", // discard all
                "P": "git.pull", // pull
                "S": "git.stageAll", // stage all
                "c": "git.commit", // commit
                "d": "git.clean", // discard
                "f": "git.fetch", // fetch
                "i": "git.init", // init
                "p": "git.push", // push
                "s": "git.stage", // stage
            },
            "o": { // options
                "s": "workbench.action.openSettingsJson", // settings
                "k": "workbench.action.openGlobalKeybindingsFile", // keysettings
                "r": "workbench.action.reloadWindow", // reload
                "S": "workbench.action.openGlobalKeybindings", // shortcuts
                "w": "editor.action.toggleRenderWhitespace", // whitespace
            },
        }
    },
    // extensions
    "C_Cpp.autoAddFileAssociations": false,
    "C_Cpp.autocomplete": "default",
    "C_Cpp.autocompleteAddParentheses": true,
    "C_Cpp.clang_format_sortIncludes": true,
    "C_Cpp.debugShortcut": false,
    "C_Cpp.default.compilerPath": "Your Path",
    "C_Cpp.enhancedColorization": "disabled",
    "code-runner.clearPreviousOutput": true,
    "code-runner.enableAppInsights": false,
    "code-runner.executorMapByGlob": {
        "*.c": "clang $fullFileName -o $fileNameWithoutExt && $fileNameWithoutExt",
        "*.cpp": "clang++ $fullFileName -o $fileNameWithoutExt && $fileNameWithoutExt",
        "*.cs": "dotnet run --project $workspaceRoot",
        "*.java": "javac $fullFileName && java $fileNameWithoutExt",
        "*.py": "python $fullFileName",
        "*.nim": "nim compile --run --hints:off --spellSuggest:0 $fullFileName",
        "*.nims": "nim --run --hints:off --spellSuggest:0 $fullFileName",
        "*.sh": "sh $fullFileName",
        "makefile": "make $fullFileName"
    },
    "code-runner.fileDirectoryAsCwd": true,
    "code-runner.ignoreSelection": true,
    "code-runner.saveAllFilesBeforeRun": true,
    "code-runner.saveFileBeforeRun": true,
    "code-runner.showRunCommandInEditorContextMenu": false,
    "code-runner.showRunCommandInExplorerContextMenu": false,
    "code-runner.showRunIconInEditorTitleMenu": false,
    "code-runner.showStopIconInEditorTitleMenu": false,
    "command-runner.terminal.autoClear": false,
    "command-runner.terminal.autoFocus": true,
    "command-runner.terminal.cwd": "${fileDirname}",
    "command-runner.terminal.name": "script",
    "csharp.referencesCodeLens.enabled": false,
    "csharp.semanticHighlighting.enabled": true,
    "errorLens.borderRadius": "3px",
    "errorLens.delay": 100,
    "errorLens.enabled": true,
    "errorLens.enabledInMergeConflict": true,
    "errorLens.enableOnDiffView": true,
    "errorLens.followCursor": "allLines",
    "errorLens.gutterIconsEnabled": true,
    "errorLens.gutterIconSet": "circle",
    "errorLens.messageBackgroundMode": "message",
    "errorLens.messageTemplate": "$count $severity: $message",
    "errorLens.onSave": false,
    "errorLens.padding": "0px 10px 0px 0px",
    "errorLens.removeLinebreaks": false,
    "errorLens.scrollbarHackEnabled": false,
    "hexeditor.columnWidth": 16,
    "hexeditor.defaultEndianness": "little",
    "hexeditor.inspectorType": "aside",
    "hexeditor.showDecodedText": true,
    "java.inlayHints.parameterNames.enabled": "none",
    "license.author": "Your Name",
    "license.default": "bsd-3-clause",
    "license.extension": ".md",
    "license.year": "auto",
    "liveServer.settings.donotShowInfoMsg": true,
    "liveServer.settings.donotVerifyTags": true,
    "liveServer.settings.host": "127.0.0.1",
    "liveServer.settings.port": 5500,
    "liveServer.settings.showOnStatusbar": false,
    "Lua.addonManager.enable": true,
    "Lua.codeLens.enable": true,
    "Lua.completion.autoRequire": true,
    "lua.debug.settings.console": "externalTerminal",
    "markdown.extension.list.indentationSize": "inherit",
    "markdown.extension.theming.decoration.renderCodeSpan": true,
    "omnisharp.analyzeOpenDocumentsOnly": false,
    "omnisharp.autoStart": true,
    "omnisharp.enableMsBuildLoadProjectsOnDemand": true,
    "omnisharp.enableRoslynAnalyzers": true,
    "omnisharp.loggingLevel": "debug",
    "omnisharp.organizeImportsOnFormat": true,
    "omnisharp.path": "latest",
    "omnisharp.useEditorFormattingSettings": true,
    "omnisharp.useModernNet": true,
    "polacode.target": "container",
    "polacode.transparentBackground": true,
    "redhat.telemetry.enabled": false,
    "terminalAllInOne.disableAllMessages": true,
    "terminalAllInOne.script.disableDescription": true,
    "terminalAllInOne.scripts": [],
    "zig.zigPath": "Your Path",
    "zig.zls.enableInlayHints": false,
    "zig.zls.path": "Your Path",
    "zig.zls.semanticTokens": "none",
    "todohighlight.isEnable": true,
    "todohighlight.isCaseSensitive": true,
    "todohighlight.include": [
        "**/*.*"
    ],
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
            "text": "TODO",
            "color": "#f1c40f",
            "fontWeight": "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)TODO(?!\\w)"
            }
        },
        {
            "text": "FIXME",
            "color": "#e74c3c",
            "fontWeight": "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)FIXME(?!\\w)"
            }
        },
        {
            "text": "NOTE",
            "color": "#3498db",
            "fontWeight": "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)NOTE(?!\\w)"
            }
        },
        {
            "text": "HACK",
            "color": "#9b59b6",
            "fontWeight": "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)HACK(?!\\w)"
            }
        },
        {
            "text": "BUG",
            "color": "#2ecc71",
            "fontWeight": "bold",
            "backgroundColor": "#00000000",
            "regex": {
                "pattern": "(?<=^|\"|:|\\s)BUG(?!\\w)"
            }
        }
    ],
    // sync
    "settingsSync.ignoredSettings": [
        "-C_Cpp.default.compilerPath",
        "zig.zigPath",
        "zig.zls.path"
    ],
    // settings
    "breadcrumbs.enabled": false,
    "breadcrumbs.filePath": "off",
    "breadcrumbs.icons": true,
    "debug.console.closeOnEnd": true,
    "debug.openDebug": "neverOpen",
    "debug.saveBeforeStart": "allEditorsInActiveGroup",
    "debug.terminal.clearBeforeReusing": true,
    "diffEditor.codeLens": true,
    "diffEditor.wordWrap": "inherit",
    "editor.autoClosingBrackets": "always",
    "editor.autoClosingQuotes": "always",
    "editor.autoIndent": "full",
    "editor.bracketPairColorization.enabled": false,
    "editor.codeLens": true,
    "editor.colorDecorators": true,
    "editor.cursorBlinking": "smooth",
    "editor.cursorStyle": "block",
    "editor.cursorWidth": 3,
    "editor.definitionLinkOpensInPeek": false,
    "editor.detectIndentation": true,
    "editor.dragAndDrop": false,
    "editor.emptySelectionClipboard": true,
    "editor.fastScrollSensitivity": 5,
    "editor.find.seedSearchStringFromSelection": "selection",
    "editor.folding": true,
    "editor.foldingHighlight": false,
    "editor.foldingStrategy": "auto",
    "editor.fontFamily": "Cascadia Mono, Jetbrains Mono, Source Code Pro",
    "editor.fontLigatures": false,
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
    "editor.letterSpacing": 0,
    "editor.lightbulb.enabled": false,
    "editor.lineHeight": 22,
    "editor.lineNumbers": "on",
    "editor.linkedEditing": false,
    "editor.links": true,
    "editor.matchBrackets": "always",
    "editor.minimap.enabled": false,
    "editor.overviewRulerBorder": false,
    "editor.padding.bottom": 1,
    "editor.padding.top": 1,
    "editor.quickSuggestionsDelay": 0,
    "editor.renderLineHighlight": "all",
    "editor.renderWhitespace": "none",
    "editor.scrollBeyondLastColumn": 4,
    "editor.scrollBeyondLastLine": false,
    "editor.showFoldingControls": "always",
    "editor.smoothScrolling": false,
    "editor.suggest.filterGraceful": true,
    "editor.suggest.insertMode": "replace",
    "editor.suggest.localityBonus": true,
    "editor.suggest.matchOnWordStartOnly": true,
    "editor.suggest.preview": false,
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
    "files.defaultLanguage": "${activeEditorLanguage}",
    "files.enableTrash": true,
    "files.encoding": "utf8",
    "files.eol": "\n",
    "files.exclude": {
        "**/.godot": true,
        "**/.config": true,
        "**/.git": true,
        "**/.vs": true,
        "**/bin": true,
        "**/obj": true
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
    "terminal.integrated.customGlyphs": true,
    "terminal.integrated.defaultProfile.windows": "PowerShell",
    "terminal.integrated.enableFileLinks": "on",
    "terminal.integrated.gpuAcceleration": "on",
    "terminal.integrated.shellIntegration.enabled": true,
    "terminal.integrated.showLinkHover": true,
    "terminal.integrated.tabFocusMode": false,
    "window.commandCenter": false,
    "window.confirmBeforeClose": "keyboardOnly",
    "window.dialogStyle": "custom",
    "window.enableMenuBarMnemonics": false,
    "window.experimental.windowControlsOverlay.enabled": true,
    "window.menuBarVisibility": "hidden",
    "window.title": "${rootName}",
    "window.titleBarStyle": "custom",
    "window.zoomLevel": 0.8,
    "workbench.activityBar.visible": false,
    "workbench.commandPalette.experimental.suggestCommands": true,
    "workbench.editor.enablePreview": false,
    "workbench.editor.showTabs": true,
    "workbench.editor.tabCloseButton": "off",
    "workbench.editor.tabSizing": "shrink",
    "workbench.iconTheme": "material-icon-theme",
    "workbench.startupEditor": "none",
    "workbench.statusBar.visible": false,
    "workbench.colorTheme": "Yellowed",
}
~~~

### :keyboard: Keybindings
~~~json with comments
[
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
    {
        "key": "tab",
        "command": "selectNextSuggestion",
        "when": "suggestWidgetMultipleSuggestions && suggestWidgetVisible && textInputFocus"
    },
]
~~~
