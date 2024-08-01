# 校园悬浮窗Win32插件示例
适用于校园悬浮窗3.5版本以上的插件示例
## 文件说明
| 文件名 | 文件说明 |
| ----- | ---------|
| `exec` | 存放关于插件的win32应用程序的文件夹（可自定义文件名和内容）|
| `icon.png/logo.png` | 插件图标（可自定义文件名和内容） |
| `pluginConfig.json` | 必须，插件的配置文件（写法见下文）|
## 配置文件说明
配置文件为插件目录下的`pluginConfig.json`文件，遵循json写法，以下是项目中的`pluginConfig.json`文件，下文将逐一解释。
```json
{
    "name": "Notepad",
    "type":"win32",
    "execPath": "exec/youdao.exe",
    "icon":"logo.png",
    "pluginVersion": "1.0",
    "pluginAuthor":"Aero8m",
    "pluginIntroduce":"校园悬浮窗的win32应用插件示例"
}
```
| 字段 | 字段类型 | 字段说明 |
| --- | -------- | --------- |
| `name` | `String` | 插件名称 |
| `type` | `String` | 插件的类型，仅可填`win32`、`html`、`url` |
| `execPath` | `String` | 插件主程序的相对路径 |
|  `icon` | `String` | 插件图标的相对路径 |
| `pluginVersion` | `String` | 插件版本 |
| `pluginAuthor` | `String` | 插件作者 |
| `pluginIntroduce` | `String` | 插件简介 |

## 打包说明
打包需打包为普通zip格式，注意，不能只打包插件的文件，需将把插件文件夹一起打包
