## ZSH

```bash
    # 01 install ZSH
    sudo apt install zsh -y

    # 02 install POWERLINE
    sudo apt install powerline fonts-powerline

    # 03
    chsh -s /bin/zsh

    # 04 Install oh-my-zsh via curl
    sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

    # 05 Zsh Syntax Highlighting
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    
     # 06 Zsh Auto Suggestions
     git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

    # 07 Spaceship Prompt
    git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1

        # Link
        ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"

    # 04 Edit .zshrc
    code ~/.zshrc

        # Change
        ZSH_THEME="spaceship"
        plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

```

## Visual Studio Code

```json
{
  // "terminal.integrated.shell.linux": "/bin/zsh",
  // "terminal.integrated.shell.osx": "/bin/zsh",
  "[json]": {
    "editor.quickSuggestions": {
      "strings": true
    },
    "editor.suggest.insertMode": "replace",
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "explorer.compactFolders": false,
  "workbench.colorTheme": "Dracula Soft",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.startupEditor": "newUntitledFile",
  "editor.tabSize": 2,
  "explorer.confirmDelete": false,
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  },
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "njk": "html"
  },
  "explorer.confirmDragAndDrop": false,
  "editor.formatOnSave": true,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "launch": {
    "configurations": [],
    "compounds": []
  },
  "files.associations": {
    "*.html": "html"
  },
  "material-icon-theme.files.associations": {
    "*.html": "html",
    "ormconfig.json": "database",
    "tsconfig.json": "tune"
  },
  "material-icon-theme.folders.associations": {
    "infra": "app",
    "entities": "class",
    "shemas": "class",
    "typeorm": "database",
    "repositories": "mappings",
    "http": "container",
    "migrations": "tools",
    "modules": "components",
    "implementations": "core",
    "dtos": "typescript",
    "fakes": "mock",
    "schemas": "class"
  },
  "liveServer.settings.donotShowInfoMsg": true,
  "eslint.alwaysShowStatus": true,

  "git.enableSmartCommit": true,
  "editor.fontSize": 15,
  "editor.formatOnType": false,
  "prettier.singleQuote": true,
  "prettier.semi": false,
  "javascript.updateImportsOnFileMove.enabled": "never",
  "typescript.updateImportsOnFileMove.enabled": "never",
  "cSpell.userWords": [],
  "workbench.editor.enablePreview": false,

  "terminal.integrated.tabs.enabled": true,
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,

  "editor.minimap.maxColumn": 80,
  "editor.inlineSuggest.enabled": true,
  "github.copilot.enable": {
    "*": false,
    "yaml": false,
    "plaintext": false,
    "markdown": false,
    "typescriptreact": false
  },
  "git.confirmSync": false,
  "extensions.ignoreRecommendations": true,
  "editor.suggestSelection": "first",
  "files.exclude": {
    "**/.classpath": true,
    "**/.project": true,
    "**/.settings": true,
    "**/.factorypath": true
  },
  "redhat.telemetry.enabled": true,
  "workbench.editorAssociations": {
    "*.class": "default"
  },

  "window.zoomLevel": 1,
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascript]": {
    "editor.defaultFormatter": "vscode.typescript-language-features"
  },
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "bracketPairColorizer.depreciation-notice": false,
  "security.workspace.trust.untrustedFiles": "open"
}
```

### Links

- [Oh My ZSH](https://ohmyz.sh/)
- [Spaceship Prompt](https://github.com/spaceship-prompt/spaceship-prompt)
- [Zsh Auto Suggestions](https://github.com/zsh-users/zsh-autosuggestions)
- [Zsh Syntax Highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md/)
