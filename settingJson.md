// {
//   "git.autofetch": true,
//   "[scss]": {
//     "editor.defaultFormatter": "esbenp.prettier-vscode"
//   },
//   "[javascriptreact]": {
//     "editor.defaultFormatter": "esbenp.prettier-vscode"
//   },
//   "notebook.formatOnSave.enabled": true,
//   "editor.defaultFormatter": "esbenp.prettier-vscode",
//   "editor.formatOnSave": true,
//   "editor.formatOnPaste": true,
//   "[prisma]": {
//     "editor.defaultFormatter": "Prisma.prisma"
//   },
//   "workbench.colorTheme": "GitHub Dark Colorblind (Beta)",
//   "terminal.integrated.env.windows": {},
//   "console-ninja.featureSet": "Community",
//   "prisma.showPrismaDataPlatformNotification": false,
//   "editor.fontSize": 13,
//   "debug.console.fontSize": 13,
//   "terminal.integrated.fontSize": 12,
//   "chat.editor.fontSize": 12,
//   "workbench.iconTheme": "file-icons",
//   "liveServer.settings.donotVerifyTags": true,
//   "liveServer.settings.donotShowInfoMsg": true,
//   "workbench.startupEditor": "readme",
//   "terminal.integrated.cursorStyle": "line",
//   "terminal.integrated.defaultProfile.windows": "Git Bash"
// }

{
  "git.autofetch": true,
  // Workbench & Window Styling
  "workbench.iconTheme": "vs-minimal",
  // "workbench.colorTheme": "Visual Studio Dark",
  // "workbench.editor.tabSizing": "shrink",
  "window.titleBarStyle": "custom",
  "window.title": "${dirty}${activeEditorShort}${separator}${rootName}",

  //editor styling
  "editor.formatOnSave": true,
  "editor.formatOnType": false,
  "editor.formatOnPaste": false,
  "editor.wordWrap": "on",
  "window.zoomLevel": 0,
  "editor.fontFamily": "'Cascadia Code', monospace",
  "editor.fontLigatures": true,
  "editor.fontSize": 13,
  "editor.lineHeight": 22,
  "editor.letterSpacing": 0.1,
  "editor.cursorWidth": 3,
  "editor.cursorBlinking": "smooth",
  "editor.cursorStyle": "line",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.smoothScrolling": true,
  "editor.minimap.enabled": true,
  "editor.minimap.renderCharacters": false,
  "editor.minimap.scale": 1,
  "editor.renderWhitespace": "selection",
  "editor.renderLineHighlight": "all",
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": "active",
  "editor.linkedEditing": true,
  "editor.detectIndentation": false,
  "editor.tabSize": 1,
  "editor.insertSpaces": true,
  "editor.fontWeight": "200",
  "files.autoSave": "off",
  // "files.autoSaveDelay": 1000,
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,

  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  // "javascript.format.semicolons": "insert",
  // "typescript.format.semicolons": "insert",

  //custom vscode css
  // "customizeUI.font.regular": "Inter V",
  // "customizeUI.font.monospace": "Rec Mono Duotone",
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  // Terminal Customization
  "terminal.integrated.fontFamily": "Firacode NF",
  "terminal.integrated.fontSize": 13,
  "terminal.integrated.cursorStyle": "underline",
  "terminal.integrated.cursorBlinking": true,
  "terminal.integrated.defaultProfile.windows": "Git Bash",
  "terminal.integrated.env.windows": {
    "PSICON": "😁"
  },
  "react-native-tools.showUserTips": false,
  "javascript.validate.enable": false,
  "javascript.updateImportsOnFileMove.enabled": "always",
  // "[typescript]": {
  //   "editor.defaultFormatter": "esbenp.prettier-vscode"
  // },
  "typescript.updateImportsOnFileMove.enabled": "always",
  "typescript.preferences.importModuleSpecifier": "relative",
  "typescript.suggestionActions.enabled": true,
  "typescript.format.enable": true,
  "diffEditor.ignoreTrimWhitespace": false,
  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features"
  },
  "liveServer.settings.donotShowInfoMsg": true,
  "jshint.enable": false,
  "[typescriptreact]": {
    "editor.defaultFormatter": "vscode.typescript-language-features"
  },
  "[json]": {
    "editor.defaultFormatter": "vscode.json-language-features"
  },
  "editor.inlineSuggest.enabled": true,
  "prettier.useEditorConfig": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "never",
    "source.organizeImports": "never",
    "source.fixAll": "never"
  },
  "eslint.validate": ["javascript"],
  "[vue]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  // "powershell.powerShellDefaultVersion": "Windows PowerShell (x64)",
  // "workbench.colorTheme": "underdark-jungle",
  "diffEditor.codeLens": true,
  "workbench.colorCustomizations": {
    "activityBar.activeBackground": "#cdbc70",
    "activityBar.activeBorder": "#f0f094",
    "activityBar.foreground": "#c19f9f",
    "activityBar.inactiveForeground": "#7d6a19",
    "activityBarBadge.background": "#83790c",
    "activityBarBadge.foreground": "#ffffff",
    "sash.hoverBorder": "#7e6e2a",
    "statusBar.foreground": "#ffffff",
    "statusBarItem.hoverBackground": "#7e6e2a",
    "statusBarItem.remoteBackground": "#ccaa13",
    "statusBarItem.remoteForeground": "#644848",
    "titleBar.activeBackground": "#2a2a16f6",
    "titleBar.activeForeground": "#ffffff",
    "titleBar.inactiveBackground": "#201e1e",
    "titleBar.inactiveForeground": "#928f8f",
    "editor.background": "#000000",
    "sideBar.background": "#1a1801",
    "statusBar.background": "#1a1506",
    "activityBar.background": "#414817",
    "terminal.background": "#332e12",
    "editorGutter.background": "#38393a73",
    "editor.lineHighlightBackground": "#494d4955",
    "editor.selectionBackground": "#dbdb2040",
    "editorCursor.foreground": "#d9ff00",
    "editorWhitespace.foreground": "#485a3a",
    "editorIndentGuide.activeBackground1": "#edff4d",
    "editor.lineHighlightBorder": "#b4d92f4c"
  },

  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": ["comment", "comment.line", "comment.block"],
        "settings": {
          "fontStyle": "italic",
          "foreground": "#aaa5a5"
        }
      },
      {
        "scope": ["string", "string.quoted"],
        "settings": {
          "foreground": "#e6b0b0"
        }
      },
      {
        "scope": ["keyword", "keyword.control"],
        "settings": {
          "foreground": "#45706e",
          "fontStyle": "bold"
        }
      },
      {
        "scope": ["entity.name.function", "support.function"],
        "settings": {
          "foreground": "#fcc708"
        }
      },
      {
        "scope": ["variable", "variable.parameter"],
        "settings": {
          "foreground": "#62ff07"
        }
      }
    ]
  },
  "workbench.productIconTheme": "Default",
  "[scss]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "workbench.sideBar.location": "right",
  "[javascriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "workbench.activityBar.location": "top",
  "editor.codeActions.triggerOnFocusChange": true,
  "[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "github.copilot.enable": {
    "*": false,
    "plaintext": false,
    "markdown": false,
    "scminput": false
  }
}
