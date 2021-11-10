<h3 align="center">👋 Hi! This is my vscode configuration</h3>
<p align="center">
  <a href="https://gael-lopes-da-silva.github.io/MyPortfolio/">Website</a>
</p>

---

<p align="center">⌨️ I use vim keybindings with the amVim extension. I have used the <a href="https://marketplace.visualstudio.com/items?itemName=vscodevim.vim">Vim</a> vscode extension by the past, but the performences issues made me changes for amVim.</p>

<p align="center">📖 I generaly use <kbd>F5</kbd> to run code with Code Runner, but I also use <kbd>F6</kbd> tu run nim code.</p>

---

### Screenshots
![](screenshots/Screenshot1.png)
![](screenshots/Screenshot2.png)

### Font
- [Cascadia Code](https://github.com/microsoft/cascadia-code)

### Extensions
- [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
- [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
- [C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp)
- [Code Autocomplete](https://marketplace.visualstudio.com/items?itemName=svipas.code-autocomplete)
- [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
- [Dark Github Markdown Preview](https://marketplace.visualstudio.com/items?itemName=ozaki.markdown-github-dark)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [French Language Pack for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=MS-CEINTL.vscode-language-pack-fr)
- [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
- [Jupyter Keymap](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter-keymap)
- [Jupyter Notebook Renderers](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter-renderers)
- [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)
- [Markdown Checkboxes](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-checkbox)
- [Markdown Emoji](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-emoji)
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
- [Monokai Accents](https://marketplace.visualstudio.com/items?itemName=tw.monokai-accent)
- [Nim](https://marketplace.visualstudio.com/items?itemName=nimsaem.nimvscode)
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [Visual Studio IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)
- [amVim](https://marketplace.visualstudio.com/items?itemName=auiworks.amvim)

### Keyboard shortcuts help
- <kbd>ctrl</kbd> + <kbd>shift</kbd> + <kbd>e</kbd>
  - Open the explorer in the activity bar.
- <kbd>ctrl</kbd> + <kbd>shift</kbd> + <kbd>x</kbd>
  - Open the extension panel in the activity bar.
- <kbd>ctrl</kbd> + <kbd>shift</kbd> + <kbd>g</kbd>
  - Open the git panel in the activity bar.
- <kbd>ctrl</kbd> + <kbd>shift</kbd> + <kbd>d</kbd>
  - Open the debuger in the activity bar.
- <kbd>ctrl</kbd> + <kbd>b</kbd>
  - Open or close the activity bar.
- <kbd>ctrl</kbd> + <kbd>p</kbd>
  - Open a menu where you can choose a file (from your folder) to open.
- <kbd>ctrl</kbd> + <kbd>w</kbd>
  - Close the selected file.
- <kbd>ctrl</kbd> + <kbd>tab</kbd>
  - Move between opened files.
- <kbd>ctrl</kbd> + <kbd>k</kbd> and <kbd>ctrl</kbd> + <kbd>o</kbd>
  - Open a folder.

### Settings
```json
{
  // options
  "editor.suggestSelection": "first",
  "editor.autoIndent": "full",
  "editor.autoClosingBrackets": "always",
  "files.autoSave": "afterDelay",
  "editor.quickSuggestionsDelay": 0,
  "debug.openDebug": "neverOpen",
  "debug.internalConsoleOptions": "openOnSessionStart",
  "debug.saveBeforeStart": "allEditorsInActiveGroup",
  "debug.terminal.clearBeforeReusing": true,
  "security.workspace.trust.enabled": false,
  "editor.suggest.showFiles": true,
  "explorer.confirmDelete": false,
  "editor.suggest.showFolders": true,
  "editor.suggest.showIcons": true,
  "editor.linkedEditing": true,
  "workbench.editor.enablePreview": false,
  "editor.detectIndentation": true,
  "workbench.editorAssociations": {
    "*.ipynb": "jupyter-notebook"
  },
  // apparence
  "workbench.activityBar.visible": false,
  "window.title": "${dirty}${activeEditorShort}${separator}${appName}",
  "editor.cursorWidth": 3,
  "editor.lineHeight": 24,
  "editor.fontFamily": "Cascadia Code, monospace",
  "terminal.integrated.fontFamily": "Cascadia Code, monospace",
  "debug.console.fontFamily": "Cascadia Code, monospace",
  "errorLens.fontFamily": "Cascadia Code, monospace",
  "editor.codeLensFontFamily": "Cascadia Code, monospace",
  "editor.fontLigatures": true,
  "editor.fontSize": 17,
  "editor.cursorBlinking": "smooth",
  "editor.cursorSmoothCaretAnimation": true,
  "editor.renderWhitespace": "selection",
  "workbench.editor.tabCloseButton": "off",
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
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Monokai +Blue",
  // syncronisation
  "settingsSync.ignoredSettings": [
    "python.pythonPath",
  ],
  "settingsSync.ignoredExtensions": [
    "neikeq.godot-csharp-vscode",
    "geequlim.godot-tools",
    "ms-vscode.mono-debug",
    "terminal.integrated.fontfamily"
  ],
  // extensions
  "errorLens.gutterIconsEnabled": true,
  "errorLens.delay": 1,
  "errorLens.followCursor": "closestProblem",
  "code-runner.clearPreviousOutput": true,
  "code-runner.ignoreSelection": true,
  "code-runner.runInTerminal": false,
  "code-runner.fileDirectoryAsCwd": true,
  "code-runner.preserveFocus": true,
  "code-runner.executorMap": {
    "javascript": "node",
    "java": "cd $dir && javac $fileName && java $fileNameWithoutExt",
    "c": "gcc $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
    "cpp": "g++ $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
    "objective-c": "cd $dir && gcc -framework Cocoa $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
    "php": "php",
    "python": "python -u $fileName",
    "perl": "perl",
    "perl6": "perl6",
    "ruby": "ruby",
    "go": "go run",
    "lua": "lua",
    "groovy": "groovy",
    "powershell": "powershell -ExecutionPolicy ByPass -File",
    "bat": "cmd /c",
    "shellscript": "bash",
    "fsharp": "fsi",
    "csharp": "dotnet run",
    "vbscript": "cscript //Nologo",
    "typescript": "ts-node",
    "coffeescript": "coffee",
    "scala": "scala",
    "swift": "swift",
    "julia": "julia",
    "crystal": "crystal",
    "ocaml": "ocaml",
    "r": "Rscript",
    "applescript": "osascript",
    "clojure": "lein exec",
    "haxe": "haxe --cwd $dirWithoutTrailingSlash --run $fileNameWithoutExt",
    "rust": "cd $dir && rustc $fileName && $dir$fileNameWithoutExt",
    "racket": "racket",
    "scheme": "csi -script",
    "ahk": "autohotkey",
    "autoit": "autoit3",
    "dart": "dart",
    "pascal": "cd $dir && fpc $fileName && $dir$fileNameWithoutExt",
    "d": "cd $dir && dmd $fileName && $dir$fileNameWithoutExt",
    "haskell": "runhaskell",
    "nim": "nim c -r --verbosity:2 --hints:off $fileName",
    "lisp": "sbcl --script",
    "kit": "kitc --run",
    "v": "v run",
    "sass": "sass --style expanded",
    "scss": "scss --style expanded",
    "less": "cd $dir && lessc $fileName $fileNameWithoutExt.css",
    "FortranFreeForm": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
    "fortran-modern": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
    "fortran_fixed-form": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
    "fortran": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt"
  },
  "notebook.lineNumbers": "on",
  "nim.enableNimsuggest": true,
  "nim.nimprettyIndent": 2,
  "tabnine.enable": true,
  "amVim.useSystemClipboard": true,
  "csharp.referencesCodeLens.enabled": false,
  "git.autofetch": true,
  "git.enableSmartCommit": true,
  "git.confirmSync": false,
  "jupyter.askForKernelRestart": false,
}
```

### Keybindings
```json
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
        "command": "tab",
        "when": "editorTextFocus && !editorTabMovesFocus"
    },
    {
        "key": "shift+tab",
        "command": "outdent",
        "when": "editorTextFocus && !editorTabMovesFicus"
    },
    {
        "key": "ctrl+b",
        "command": "workbench.action.toggleSidebarVisibility"
    },
]
```