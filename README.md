# vscode_lovely_shortcut
Perfence lovely shortcode in linux

### Detail

- 1) ``` ctrl +shift +p```
  2) Open home/{user}/.config/Code/User/keybindings.json
  3) paste this
    ```json
    // Place your key bindings in this file to override the defaults
[
    
        {
            "key": "ctrl+c",
            "command": "workbench.action.terminal.copySelection",
            "when": "terminalFocus"
        },
        {
            "key": "ctrl+c",
            "command": "workbench.action.terminal.sendSequence",
            "args": { "text": "\u0003" },
            "when": "terminalFocus && !terminalTextSelected"
        },
        {
            "key": "ctrl+v",
            "command": "workbench.action.terminal.paste",
            "when": "terminalFocus"
        },
        {
            "key": "ctrl+a",
            "command": "workbench.action.terminal.selectAll",
            "when": "terminalFocus"
        },
        
         {
            // Ctrl+Left Arrow → previous editor
            "key": "ctrl+left",
            "command": "workbench.action.previousEditorInGroup"
       },
       {
           // Ctrl+Right Arrow → next editor
           "key": "ctrl+right",
           "command": "workbench.action.nextEditorInGroup"
       }
    
]
    ```
