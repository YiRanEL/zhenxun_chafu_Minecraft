# ✨ Minecraft_server_check_plugins for [zhenxun_bot](https://github.com/hibikier/zhenxun_bot)

[Nonebot Version](https://github.com/molanp/nonebot_plugin_mccheck/)

English|[简体中文](README.md)

## 🤔 If you have any good functional suggestions, please put forward them in [Issues](https://github.com/molanp/zhenxun_chafu_Minecraft/issues)

## 📈 Implemented functions

- [x] IPv6 supported
- [x] Full platform adapter support
- [x] Adapted unicode full fonts and glyphs
- [x] Render Motd styles
- [x] Query server nickname
- [x] Query the maximum number of servers, the current number of players and player list
- [x] Query server motd
- [x] returns the server address and port
- [x] Returns the server online status
- [x] Query server latency
- [x] More precise delay
- [x] Double-query on the interworking server is supported
- [x] Error message feedback
- [x] Port autocompletion
- [x] Wisdom can determine whether the IP address is correct
- [x] Does not depend on any external API :)
- [x] Support special port queries (e.g. `2`, `80`, `443` etc.)
- [x] Query server favicon
- [x] Multilingual
- [x] SRV support 
- [x] Fully colored underlined/strikethrough
- [x] Get server protocol number

## 📑 Future functions

- [ ] And more...

## 🖼️ Renderings

v1.24

![Image_31020983743694.png](https://github.com/user-attachments/assets/2db47c9a-7ba1-4ce7-a31c-b65f6e848308)
![Image](https://github.com/user-attachments/assets/2ca058f5-2341-425d-8033-63dad8d43fbf)

## 💿 Install

  - Put `mc_check` folder in `plugins` folder or custom folder.

## 🎉 Usage

| Command | Parameter | Scope | Description |
|:-------:|:---------:|:-----:|:-----------:|
| `mcheck` | `[ip]:[port]` or `[ip]` | Private/Group Chat | Check Minecraft server status |
| `set_lang` | Language name | Private/Group Chat | Set the language used by the plugin for rendering images |
| `lang_now` | None | Private/Group Chat | View the current language used by the plugin for rendering images |
| `lang_list` | None | Private/Group Chat | View the list of languages supported by the plugin |

### 🎈 Special Notes
Querying an IPv6 server
```
mcheck [2001:db8:85a3::8a2e:370:7334]:25565  <- IPv6 server address and port, the port and colon can be omitted
```
or
```
mcheck 2001:db8:85a3::8a2e:370:7334  <- IPv6 server address, the plugin will automatically complete the port number
```
or
```
mcheck 2001:db8:85a3::8a2e:370:7334:25565  <- IPv6 server address and port
```
or
```
mcheck [2001:db8:85a3::8a2e:370:7334]  <- IPv6服务器地址
```

## ⚙️ Configuration

| Configuration Item | Required | Default Value | Description |
|:-----:|:----:|:----:|:----:|
| `language` | False | `zh-cn` | Languages used by the plugin to render images<br>Available languages: [`zh-cn`,`zh-tw`,`en`] |
| `type` | False | `0` | The type of message the plugin sends (`0` for HTML, `1` for image, `2` for text) |

## 🎲 Comparison of message types

| Type | Special Styles | Favicon | Colored underline/strikethrough | Full Unicode font support |
|:-----:|:-----:|:-----:|:-----:|:-----:|
| Text | ❌ | ⭕ | ❌ | ⭕ |
| Picture | ⭕ | ⭕ | ⭕ | ❌ |
| HTML | ⭕ | ⭕ | ⭕ | ⭕ |

# [Download](https://github.com/molanp/zhenxun_chafu_Minecraft/releases)


## Requirement
```shell
pip install "dnspython>=2.2.1,<2.5.0"
```

## Thanks
* [minestat](https://github.com/FragLand/minestat): A multi-platform Minecraft server query module
* [@tzdtwsj](https://github.com/tzdtwsj): For the project, suggestions for image rendering function, color rendering function and implementation ideas of interoperability query scheme are proposed.
