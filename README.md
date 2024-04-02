## SSH

```bash
cd ~/.ssh

ssh-keygen -t rsa -b 4096 -C "email"

eval $(ssh-agent -s)

ssh-add
    
```

## ZSH

```bash
    # Check 
    curl --version

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
        ZSH_THEME="norm"
        plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

    # Themes

    https://github.com/ohmyzsh/ohmyzsh/wiki/Themes
    

```

## Visual Studio Code

```json
{
  // "terminal.integrated.shell.linux": "/bin/zsh",
  // "terminal.integrated.shell.osx": "/bin/zsh",

  "workbench.startupEditor": "newUntitledFile",
  "editor.fontSize": 15,
  "javascript.suggest.autoImports": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "extensions.ignoreRecommendations": true,
  "typescript.tsserver.log": "off",
  "screencastMode.onlyKeyboardShortcuts": true,
  "editor.parameterHints.enabled": false,
  "editor.renderLineHighlight": "gutter",
  "cSpell.language": "en,pt,pt_BR",
  "editor.lineHeight": 26,
  "typescript.updateImportsOnFileMove.enabled": "never",
  "editor.suggestSelection": "first",
  "explorer.confirmDelete": false,
  "gitlens.codeLens.recentChange.enabled": false,
  "typescript.suggest.autoImports": true,
  "editor.fontLigatures": true,
  "workbench.editor.labelFormat": "short",
  "liveshare.featureSet": "insiders",
  "editor.acceptSuggestionOnCommitCharacter": false,
  "explorer.compactFolders": false,
  "git.enableSmartCommit": true,
  "editor.accessibilitySupport": "off",
  "explorer.confirmDragAndDrop": false,
  "terminal.integrated.fontSize": 14,
  "terminal.integrated.fontFamily": "JetBrainsMono Nerd Font",
  "editor.semanticHighlighting.enabled": false,
  "breadcrumbs.enabled": true,
  "editor.fontFamily": "Fira Code", //"JetBrains Mono"
  "gitlens.codeLens.authors.enabled": false,
  "editor.tabSize": 2,
  "security.workspace.trust.untrustedFiles": "newWindow",
  "tabnine.experimentalAutoImports": true,
  "gitlens.codeLens.enabled": false,
  "workbench.iconTheme": "material-icon-theme",
  "polacode.transparentBackground": true,
  "polacode.target": "snippet",
  "editor.minimap.enabled": false,
  "update.mode": "start",
  "workbench.colorTheme": "Dracula Soft",
  "workbench.editor.untitled.hint": "hidden",
  "liveServer.settings.donotShowInfoMsg": true,
  "window.commandCenter": true,
  "git.openRepositoryInParentFolders": "always",
  "window.zoomLevel": 1,
  "maven.dependency.enableConflictDiagnostics": true,
  "maven.executable.preferMavenWrapper": true,
  "maven.showInExplorerContextMenu": true,
  "terminal.integrated.env.linux": {},
  "redhat.telemetry.enabled": true,

  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  },
  "editor.rulers": [80, 120],
  "files.associations": {
    "*.html": "html",
    ".sequelizerc": "javascript",
    ".stylelintrc": "json",
    "*.tsx": "typescriptreact",
    ".env.*": "dotenv",
    ".prettierrc": "json"
  },
  "[prisma]": {
    "editor.formatOnSave": true
  },
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "cSpell.enableFiletypes": [
    "!asciidoc",
    "!c",
    "!cpp",
    "!csharp",
    "!go",
    "!handlebars",
    "!haskell",
    "!jade",
    "!java",
    "!latex",
    "!php",
    "!pug",
    "!python",
    "!restructuredtext",
    "!rust",
    "!scala",
    "!scss"
  ],
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.addMissingImports": true
  },
  "eslint.validate": ["javascript", "javascriptreact", "graphql"],
  "files.exclude": {
    "**/CVS": true,
    "**/.DS_Store": true,
    "**/.hg": true,
    "**/.svn": true,
    "**/.git": true
    // "node_modules": true
  },
  "[jsonc]": {
    "editor.defaultFormatter": "vscode.json-language-features"
  },
  "[json]": {
    "editor.defaultFormatter": "vscode.json-language-features"
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
  "peacock.favoriteColors": [
    {
      "name": "Angular Red",
      "value": "#dd0531"
    },
    {
      "name": "Azure Blue",
      "value": "#007fff"
    },
    {
      "name": "JavaScript Yellow",
      "value": "#f9e64f"
    },
    {
      "name": "Mandalorian Blue",
      "value": "#1857a4"
    },
    {
      "name": "Node Green",
      "value": "#215732"
    },
    {
      "name": "React Blue",
      "value": "#61dafb"
    },
    {
      "name": "Something Different",
      "value": "#832561"
    },
    {
      "name": "Svelte Orange",
      "value": "#ff3d00"
    },
    {
      "name": "Vue Green",
      "value": "#42b883"
    },
    {
      "name": "Nest Purple",
      "value": "#b61a3d"
    }
  ],
  "totalTypeScript.hideAllTips": true,
  "totalTypeScript.hideBasicTips": true,
  "cSpell.userWords": [
    "camelcase",
    "dayjs",
    "dtos",
    "fastify",
    "jamjure",
    "Jamjuree",
    "roboto",
    "tailwindcss"
  ],
  "git.confirmSync": false
}

```

### Links

- [Oh My ZSH](https://ohmyz.sh/)
- [Spaceship Prompt](https://github.com/spaceship-prompt/spaceship-prompt)
- [Zsh Auto Suggestions](https://github.com/zsh-users/zsh-autosuggestions)
- [Zsh Syntax Highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md/)
