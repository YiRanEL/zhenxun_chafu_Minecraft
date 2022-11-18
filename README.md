# 我的世界服务器状态查询插件，适配[zhenxun_bot](https://github.com/hibikier/zhenxun_bot)
# 中文|[English](https://github.com/molanp/zhenxun_chafu_Minecraft/master/README_en.md)
## 若有什么好的功能建议，欢迎在[Issues](https://github.com/molanp/zhenxun_chafu_Minecraft/issues)中提出
***
## 已实现的功能

- [x] 查询服务器昵称
- [x] 查询服务器最大人数,当前人数
- [x] 查询服务器motd
- [x] 查询服务器favicon[无则不发送]
- [x] 返回服务器地址及端口
- [x] 返回服务器在线状态
- [x] 查询服务器延迟
- [x] 更精确的延迟
- [x] 支持UDP服务器
- [x] 错误信息反馈
- [x] 端口自动补全
- [x] 智~~障~~能判断IP地址是否正确

## 未来的功能

- [ ] 获取服务器协议号[没什么用，未开发]
- [ ] 获取服务器官网[如果存在]
- [ ] 获取服务器motd的json版本[已实现但未启用]
- [ ] 添加配置文件[技术不成熟，测试发现会有许多bug]
- [ ] 敬请期待

## 测试截图

![测试截图](https://user-images.githubusercontent.com/104612722/201504468-d9b96fdf-fca2-4200-b740-51acfc6dff4c.jpg)

此图使用v0.6版本↑
<!--图片地址：https://user-images.githubusercontent.com/104612722/201504468-d9b96fdf-fca2-4200-b740-51acfc6dff4c.jpg-->

## 使用方法
- 安装
  - 将`chafu`文件夹放入`plugins`文件夹或自定义文件夹内
  - 若提示缺少依赖，请执行`pip install ping3`~~(理论上来说必定缺少此模块)~~
- 使用
  - 查服 [ip]:[port]  {Java}
  - b查 [ip]:[port]    {基岩版}

# 下载地址

## 建议直接copy源码，releases内更新不及时
[下载地址](https://github.com/molanp/zhenxun_chafu_Minecraft/releases)

# 更新日志
<details>
<summary>更新日志</summary>

## 2022/11/14
### v0.7
统一输入格式

优化代码逻辑

规范变量名

对api调用进行限制

取消了超时判断，但可能会造成响应时间变长

若频繁报错则可能遇到了网络波动(基岩版查服api站点不稳定
)，请尝试重启bot

输入时若`ip`后若无端口(且无`:`)，自动使用默认端口[25565/19132]
## 2022/11/13
### v0.6-plus
支持发送错误信息

支持查询UDP协议服务器
### v0.6[beta内部测试]
支持查询UDP服务器,但命令冲突[已修复]
## 2022/11/12
### v0.5
更精确的服务器延迟
## 2022/11/09
### v0.4-fix[releases中第一个版本]
重命名文件
### v0.4
修复favicon不存在造成的消息发送失败问题
### v0.3
支持发送favicon

更灵敏的触发
## 2022/10/31
### vfix-0.2
更新usage
## 2022/10/25
### v0.1[标签new,初版本]
支持查询JAVA服务器

支持发送延迟

</details>
