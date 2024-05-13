# `@zhur06/prettier-config`

> My personal [Prettier](https://prettier.io) config.

## Usage

**Install**:

```bash
npm i --save-dev https://github.com/Zhur06/prettier-config
```

**Edit `package.json`**:

```jsonc
{
  // ...
  "prettier": "@zhur06/prettier-config"
}
```


# Usefull stuff for code formatting

## Add script to format

In package.json add script

```json
{
  // ...
  "scripts": {
    // ...
    "format": "npx prettier . --write"
  }
}
```

## Define vscode shortcut

- Open command pallet (`cmd` `shift` `P`)
- Write `> Preferences: open Keyboard Shortcuts (JSON)`
- Paste block with shortcut

```json
{
  // ...
  {
    "key": "alt+f",
    "command": "workbench.action.terminal.sendSequence",
    "args": {
      "text": "npm run-script format\u000D"
    }
  }
}
```
[More on keybinds](https://code.visualstudio.com/docs/getstarted/keybindings)
