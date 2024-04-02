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
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Dracula Refined",
  "editor.formatOnSave": true,
  "editor.fontFamily": "Fira Code",
  "editor.fontSize": 16,
  "chat.editor.fontSize": 16,
  "editor.lineHeight": 1.8,
  "editor.rulers": [80, 120],
  "workbench.startupEditor": "newUntitledFile",
  "editor.renderLineHighlight": "gutter",
  "editor.fontLigatures": true,
  "workbench.editor.labelFormat": "short",
  "explorer.compactFolders": false,
  "editor.semanticHighlighting.enabled": false,
  "breadcrumbs.enabled": false,
  // "editor.minimap.enabled": false,
  "editor.scrollbar.horizontal": "hidden",
  "editor.scrollbar.vertical": "hidden",
  "editor.tabSize": 2,
  "scm.inputFontSize": 15,
  "terminal.integrated.fontSize": 15,
  "debug.console.fontSize": 15,
  "markdown.preview.fontSize": 16,
  "javascript.suggest.autoImports": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "extensions.ignoreRecommendations": true,
  "typescript.tsserver.log": "off",
  "editor.parameterHints.enabled": false,
  "cSpell.language": "en,pt,pt_BR",
  "typescript.updateImportsOnFileMove.enabled": "never",
  "editor.suggestSelection": "first",
  "explorer.confirmDelete": false,
  "gitlens.codeLens.recentChange.enabled": false,
  "typescript.suggest.autoImports": true,
  "liveshare.featureSet": "insiders",
  "editor.acceptSuggestionOnCommitCharacter": false,
  "git.enableSmartCommit": true,
  "editor.accessibilitySupport": "off",
  "explorer.confirmDragAndDrop": false,
  "terminal.integrated.fontFamily": "JetBrainsMono Nerd Font",
  "gitlens.codeLens.authors.enabled": false,
  "security.workspace.trust.untrustedFiles": "newWindow",
  "gitlens.codeLens.enabled": false,
  "update.mode": "start",
  "window.commandCenter": true,
  "git.openRepositoryInParentFolders": "always",
  "terminal.integrated.env.linux": {},
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
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
    "source.fixAll.eslint": "explicit",
    "source.addMissingImports": "explicit"
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
  "git.confirmSync": false,
  "liveServer.settings.donotShowInfoMsg": true,
  "console-ninja.featureSet": "Community",
  "console-ninja.warnOnNoToolsDetected": false,
}

```

### Links

- [Oh My ZSH](https://ohmyz.sh/)
- [Spaceship Prompt](https://github.com/spaceship-prompt/spaceship-prompt)
- [Zsh Auto Suggestions](https://github.com/zsh-users/zsh-autosuggestions)
- [Zsh Syntax Highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md/)
