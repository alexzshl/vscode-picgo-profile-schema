# Picgo Profile Schema

[![vsm-version](https://img.shields.io/visual-studio-marketplace/v/alexzshl.picgo-profile-schema?style=flat-square&label=VS%20Marketplace&logo=visual-studio-code)](https://marketplace.visualstudio.com/items?itemName=alexzshl.picgo-profile-schema)

This extension provides schema for profile of picgo:
- [PicGo-Core](https://picgo.github.io/PicGo-Core-Doc/)
- [Picgo-electron](https://picgo.github.io/PicGo-Doc/)

可以简单理解为：为使用picogo-core的用户提供配置文件的代码提示，当然你必需使用vscode打开配置文件。
推荐将vscode作为json文件的默认打开方式。如果使用typora，设置中有按钮可以直接打开picgo-core配置文件。
如果有需要，后面会添加几个命令用于从vscode直接打开配置文件。

## Features

Picgo-electron users can have gui interface for configuration, but PicGo-Core users can only use the cli tool. With all due respect, it's not a good experience to configure dozens of settings with cli. So I wrote this extension to provide json schema foundation for picgo profile.

**JSON Schema** provides data validation, more importantly, we can get smart tips after opening picgo profile with VSCode.

![image-20200601183545081](./media/picgo.gif)

### Profile Path

PicGo-Core and Picgo-electron has different defalt profile path.

##### PicGo-Core

- **Windows**: `C:/Users/[user-name]/.picgo/config.json`
- **Linux**: `~/.picgo/config.json`
- **MacOS**: `~/.picgo/config.json`

##### Picgo-electron

- Windows: `C:/Users/[user-name]/AppData/Roaming/picgo/data.json`
- Linux: `$XDG_CONFIG_HOME/picgo/data.json` or `~/.config/picgo/data.json`
- macOS: `~/Library/Application/Support/picgo/data.json`

## Requirements

## Known Issues

## Contribution
[JSON Schema](http://json-schema.org/)
-----------------------------------------------------------------------------------------------------------
