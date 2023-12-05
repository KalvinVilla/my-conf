# VS Code Config

## extensions
- Material Icon Theme
- multi-command
- Prettier
- Tokyo Night
- Docker
- GitHub Copilot

## policies
- JetBrainsMono

## settings.json :
```
{
    "workbench.colorTheme": "Tokyo Night",
    "editor.minimap.enabled": false,
    "editor.formatOnSave": false,
    "editor.formatOnPaste": false,
    "editor.renderWhitespace": "trailing",
    "editor.linkedEditing": true,
    "editor.occurrencesHighlight": false,
    "editor.suggest.insertMode": "replace",
    "editor.acceptSuggestionOnCommitCharacter": false,
    "files.autoSave": "onFocusChange",
    "files.defaultLanguage": "markdown",
    "explorer.autoReveal": false,
    "explorer.confirmDragAndDrop": false,
    "workbench.tree.indent": 15,
    "workbench.tree.renderIndentGuides": "always",
    "workbench.editor.enablePreview": false,
    "emmet.triggerExpansionOnTab": true,
    "git.confirmSync": false,
    "git.enableSmartCommit": true,
    "editor.fontFamily": "'JetBrains Mono', Consolas, 'Courier New', monospace",
    "editor.fontLigatures": true,
    "workbench.iconTheme": "material-icon-theme",
    "material-icon-theme.hidesExplorerArrows": true,
    "workbench.colorCustomizations": {
        "[Tokyo Night]": {
            "editor.selectionBackground": "#3D59A1",
            "editor.selectionHighlightBackground": "#3D59A1"
        }
    },
    "multiCommand.commands": [
        {
            "command": "multiCommand.makeRoom",
            "sequence": [
                "workbench.action.toggleSidebarVisibility",
                "workbench.action.toggleActivitybarVisibility"
            ]
        }
    ],
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[javascriptreact]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[html]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "javascript.preferences.importModuleSpecifierEnding": "js",
    "typescript.preferences.importModuleSpecifierEnding": "js"
}
``` 

## keybinding.json
```
// Placer vos combinaisons de touches dans ce fichier pour remplacer les valeurs par défaut
[
    {
        "key": "alt+1",
        "command": "multiCommand.makeRoom"
    },
    {
        "key": "ctrl+d",
        "command": "editor.action.smartSelect.expand",
        "when": "editorTextFocus"
    },
    {
        "key": "ctrl+shift+d",
        "command": "editor.action.addSelectionToNextFindMatch",
        "when": "editorFocus"
    },
    {
        "key": "ctrl+p",
        "command": "workbench.action.showCommands"
    },
    {
        "key": "ctrl+o",
        "command": "workbench.action.quickOpen"
    },
    {
        "key": "ctrl+shift+o",
        "command": "revealFileInOS"
    },
    {
        "key": "ctrl+r",
        "command": "workbench.action.gotoSymbol"
    },
    {
        "key": "ctrl+n",
        "command": "explorer.newFile"
    },
    {
        "key": "ctrl+alt+f",
        "command": "editor.action.formatDocument"
    },
    {
        "key": "ctrl+t",
        "command": "workbench.action.terminal.toggleTerminal"
    },

]
```