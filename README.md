# Picgo Profile Schema

[ENGLISH](README-EN.md)

[![vsm-version](https://img.shields.io/visual-studio-marketplace/v/alexzshl.picgo-profile-schema?style=flat-square&label=VS%20Marketplace&logo=visual-studio-code)](https://marketplace.visualstudio.com/items?itemName=alexzshl.picgo-profile-schema)

这是一个 vscode 插件, 用于为以下 picgo 版本提供模式文件(schema):
- [PicGo-Core](https://picgo.github.io/PicGo-Core-Doc/)
- [Picgo-electron](https://picgo.github.io/PicGo-Doc/)

可以简单理解为：为 picogo-core/picgo-electron 的 JSON 配置文件提供代码提示!

你也可以不用安装此vscode插件, 只需要在 config.json 中 声明模式文件的地址:
```json
{
  "$schema": "https://gitee.com/alexzshl/vscode-picgo-profile-schema/raw/master/schemas/picgo-core.profile.schema.json",
  
  "picbed": {}
}
```

对于 typora 用户, 如果 vscode 是默认的 json 文件打开方式, typora 的图床配置中可以直接点击打开 picgo-core 的配置文件.

## 特性

Picgo-electron 拥有 GUI 界面, 因此可以方便地进行配置, 但是 picgo-core 目前只支持通过cli工具进行配置或者对照api文档手动修改配置文件. 此插件根据官方文档编写了模式文件, 当使用vscode打开配置文件后, 将获得配置验证和代码提示的功能. 顺便地, 也为 picgo-electron 的配置文件进行了支持.

![image-20200601183545081](./media/picgo.gif)

### 配置文件路径

PicGo-Core 和 Picgo-electron 使用不同的配置文件路径, 在不同的操作系统上也有所区别

##### PicGo-Core

- **Windows**: `C:/Users/[user-name]/.picgo/config.json`
- **Linux**: `~/.picgo/config.json`
- **MacOS**: `~/.picgo/config.json`

##### Picgo-electron

- Windows: `C:/Users/[user-name]/AppData/Roaming/picgo/data.json`
- Linux: `$XDG_CONFIG_HOME/picgo/data.json` or `~/.config/picgo/data.json`
- macOS: `~/Library/Application/Support/picgo/data.json`

## 图床
图床简介:
- 阿里云: [aliyun.md](./manual/uploaders/aliyun.md)

## 贡献

## 参考
[JSON Schema](http://json-schema.org/)
