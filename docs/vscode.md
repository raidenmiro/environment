# Install my vscode settings guide

## Extensions

Execute follow commands:

```sh
EXT=(
  csstools.postcss
  eamodio.gitlens
  bradlc.vscode-tailwindcss
  tock.vscode-css-custom-properties
  shakram02.bash-beautify
  styled-components.vscode-styled-components
  vue.vscode-typescript-vue-plugin
  mushan.vscode-paste-image
  mhutchie.git-graph
  formulahendry.auto-rename-tag
  fractalbrew.backticks
  pkief.material-icon-theme
  streetsidesoftware.code-spell-checker
  streetsidesoftware.code-spell-checker-russian
  orta.vscode-twoslash-queries
  unifiedjs.vscode-mdx
  vitaliymaz.vscode-svg-previewer
  yoavbls.pretty-ts-errors
  zixuanchen.vitest-explorer
  amandeepmittal.pug
  raunofreiberg.vesper
  github.github-vscode-theme
  antfu.theme-vitesse
  stylelint.vscode-stylelint
  rafaelmardojai.vscode-gnome-theme
  adpyke.codesnap
)

for EXTENSION in ${EXT[@]}; do
  code --install-extension $EXTENSION
done
```

## User settings

Open the user json settings in vscode and copy-paste this config here

```json
{
  "editor.minimap.enabled": false,
  "editor.renderWhitespace": "selection",
  "editor.rulers": [80],
  "eslint.run": "onSave",
  "window.titleBarStyle": "custom",
  "window.customMenuBarAltFocus": false,
  "window.enableMenuBarMnemonics": false,

  "files.associations": {
    "errors.ts": "rust",
    "errors.tsx": "rust",
    "**/test/*.errors.ts": "rust",
    ".huskyrc": "json",
    ".lintstagedrc": "json",
    ".stylelintrc": "json",
    ".posthtmlrc": "json",
    "*.css": "css",
    "*.desktop": "ini",
    "*.bu": "yaml",
    "*.ign": "json",
    "*.service": "ini",
    "*.timer": "ini"
  },

  "workbench.colorTheme": "Vitesse Light",
  "workbench.colorCustomizations": {
    "[GNOME dark]": {
      "editorRuler.foreground": "#151515"
    },
    "[Bluloco Light]": {
      "editorInlayHint.foreground": "#868686f0",
      "editorInlayHint.background": "#ff000000",
      "editorInlayHint.typeForeground": "#aaa5aaf0",
      "editorInlayHint.parameterForeground": "#fdb6fdf0"
    },
    "[Horizon]": {
      "titleBar.activeBackground": "#0a0a0e",
      "titleBar.inactiveBackground": "#0a0a0e",

      "editor.background": "#1b1e27",

      "activityBar.background": "#0a0a0e",
      "activityBar.border": "#0a0a0e",

      "sideBar.background": "#161920",
      "sideBar.border": "#161920",
      "sideBarSectionHeader.background": "#111116",

      "statusBar.background": "#0a0a0e",
      "statusBar.border": "#0a0a0e",

      "editorGroupHeader.tabsBackground": "#161920",
      "editorGroupHeader.tabsBorder": "#161920",

      "tab.activeBackground": "#0a0a0e",
      "tab.inactiveBackground": "#161920",

      "panel.background": "#161920",
      "panel.border": "#0a0a0e"
    },
  },

  "explorer.openEditors.visible": 0,
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "editor.tabSize": 2,
  "workbench.iconTheme": "vs-nomo-dark",
  "vsicons.presets.hideExplorerArrows": true,
  "workbench.panel.defaultLocation": "bottom",
  "javascript.updateImportsOnFileMove.enabled": "always",

  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[json]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "emmet.includeLanguages": {
    "postcss": "css"
  },

  "editor.suggestSelection": "first",
  "editor.wordSeparators": "`~!@#%^&*()-=+[{]}\\|;:'\",.<>/?",
  "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
  "editor.formatOnSave": true,
  "workbench.startupEditor": "none",
  "files.autoSave": "afterDelay",
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "terminal.integrated.defaultProfile.linux": "zsh",
  "typescript.updateImportsOnFileMove.enabled": "always",
  
  "cSpell.language": "en,ru",
  "cSpell.userWords": [
    "actix",
    "astro",
    "clsx",
    "commitlint",
    "depcruise",
    "endregion",
    "esbuild",
    "fullname",
    "inputmode",
    "linaria",
    "Nanostores",
    "patronum",
    "pixijs",
    "pnpm",
    "raidenmiro",
    "reatom",
    "sqlx",
    "Tailwindcss",
    "typewind"
  ],

  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
  ],
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "redhat.telemetry.enabled": true,
  "vsicons.dontShowNewVersionMessage": true,
  "mergeEditor.diffAlgorithm": "advanced",
  
  "tailwindCSS.experimental.classRegex": [
    ["cva\\(([^)]*)\\)", "[\"'`]([^\"'`]*).*?[\"'`]"],
  ],

  "svg.preview.transparencyGrid": false,
  "svg.preview.boundingBox": true,
  "window.menuBarVisibility": "compact",
  "workbench.statusBar.visible": false,

  "editor.fontLigatures": true,
  "editor.fontFamily": "iosevka",
  "editor.fontSize": 12,
  "editor.lineHeight": 16,
  "editor.fontVariations": "'wdth' 87.5, 'wght' 450",
  "editor.fontWeight": "500",

  "terminal.integrated.fontFamily": "iosevka",
  "terminal.integrated.fontSize": 11,
  "terminal.integrated.fontWeight": "300",
  "terminal.integrated.tabs.location": "left",

  "editor.cursorSmoothCaretAnimation": "on",
  "editor.cursorSurroundingLines": 15,
  "editor.cursorBlinking": "expand",

  "window.zoomLevel": 1,

  "breadcrumbs.enabled": false,
  "window.commandCenter": true,
  "git.mergeEditor": true,
  "git.confirmSync": false,
  "diffEditor.ignoreTrimWhitespace": false,
  "git.suggestSmartCommit": false,
  "files.exclude": {
    "**/.git": false
  },
}

```
