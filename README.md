## Extensions

Extensions are useful to help automate tasks and can also add specific and essential features of a language or framework.

| Name | Language | URL |
| ------ | ------ | ------ |
| Beautify | CSS, HTML, JS, JSON and SASS | <https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify> |
| Bracket Pair Colorizer | All | <https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer> |
| EditorConfig for VS Code | All | <https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig> |
| IntelliSense for CSS class names in HTML | [Check here](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion#supported-language-modes) | <https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion> |
| Visual Studio IntelliCode | C#, C++, JS, TS, XAML | <https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode> |


## Terminal (*only Microsft Windows*)

[Cmder](https://cmder.net/) is an excellent alternative to the native Windows terminal, it allows the use of UNIX commands (`ls`, `mv`, `rm`, `ps` and others), auto-complete and commands history.  

<a id="how-to-open-settings-json"></a>
- Open __User Settings__ in the command palette (`Ctrl` + `Shift` + `P`) > __Preferences: Open Settings (JSON)__.

File: `settings.json` <= [how to open](#how-to-open-settings-json)

Defining as integrated default terminal.


```json
"terminal.integrated.shell.windows": "cmd.exe",
"terminal.integrated.shellArgs.windows": [
    "/k",
    "%CMDER_PATH%\\vendor\\bin\\vscode_init.cmd"
]
```

> - Please download the full version of *Cmder*.
> - Don't forget to change `CMDER_ROOT` by the *Cmder* installation path.

## Fonts

Some fonts recommended to provide a better code reading experience.

File: `settings.json` <= [how to open](#how-to-open-settings-json)

- __[Fira Code](https://github.com/tonsky/FiraCode)__
```json
"editor.fontFamily": "'Fira Code'",
"editor.fontLigatures": true
```
- __[JetBrains Mono](https://www.jetbrains.com/lp/mono)__ (*my preference*)

```json
"editor.fontFamily": "'JetBrains Mono'",
"editor.fontLigatures": true
```

## Extras

File: `settings.json` <= [how to open](#how-to-open-settings-json)

```json
"git.autofetch": true,
"javascript.updateImportsOnFileMove.enabled": "always",
"vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue"
```

License
----
MIT