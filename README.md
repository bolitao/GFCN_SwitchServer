# 「少女前线」跨服手册（散爆版）（前言）
 > By: [Mornwind](https://github.com/Mornwind)
 > 
 > GitHub Link: [Mornwind/GFCN_SwitchServer](https://github.com/Mornwind/GFCN_SwitchServer) 
 > 
 > 少前跨服 - QQ 群：[`915089623`](https://jq.qq.com/?_wv=1027&k=5rnvPAT)

## 致谢

- **参考&协助**
  - [霞ヶ丘詩羽x](https://space.bilibili.com/455501)：[B站专栏（cv3630717）](https://www.bilibili.com/read/cv3630717)

---

## ⚠️ 注意事项 ⚠️

1. 本项目内所提到的所有客户端与服务器，均为**国服**。
2. 跨服脚本中**并未含有**用于修改游戏内数据以获得不正当收益的作弊内容，只是用来切换服务器，故理论上不会被封号。跨服脚本代码**公开透明**地存放于本项目中，欢迎随时进行检查。如若不放心，还请另寻他法。
3. **无法在 iOS 端进行跨服充值，否则 1000% 会错充进 iOS 官服，切记！**
4. iOS 端跨渠道混服，可参照跨 Bilibili 服的方法。

---

## iOS 端常见跨服方式

在 iOS 端上，常见的游戏跨服方式主要可分为以下三大类六小类：

| 类型 | 方式 | 优点 | 缺点 |
| :-: | :-: | :-: | :-: |
| A-1 | 通过**使用网络调试工具**，<br/>**在本地重写客户端请求**，<br/>**直接**实现跨服 | 本地修改无需依赖他人<br/>基本不受游戏版本更新影响 | 需要会亿点操作<br/>部分工具价格较高<br/>部分工具在国区无法下载 |
| A-2 | 通过**使用他人提供的代理服务器**，<br/>**在远端重写客户端请求**，<br/>**直接**实现跨服 | 操作较少 | 依赖代理服务器的稳定性<br/>安全性无法保证 |
| B-1 | 通过**对游戏客户端修改后重新打包**，<br/>**由他人统一签名后在线下载安装**，<br/>**直接**实现跨服 | 几乎无需操作 | 签名所需证书费较贵<br/>更新后需等待新跨服包发布 |
| B-2 | 通过**对游戏客户端修改后重新打包**，<br/>**自行签名然后越狱安装或侧载**，<br/>**直接**实现跨服 | 无需花钱 | 需要会亿点操作<br/>越狱影响系统安全性<br/>每 7 天需重新签名<br/>更新后需等待新跨服包发布 |
| C-1 | 通过**使用云游戏平台**，<br/>**将游戏画面实时传输至移动设备**，<br/>**间接**实现跨服 | 操作较少<br/>能跨部分渠道服 | 可选渠道服受制于云平台<br/>严重依赖网络质量<br/>安全性无法保证<br/>非会员每日游戏时长受限<br/>非会员每次进入需排队等候 |
| C-2 | 通过**使用云主机**，<br/>**将游戏画面实时传输至移动设备**，<br/>**间接**实现跨服 | 能跨渠道服 | 需要会亿点操作<br/>云主机普遍价格很高<br/>严重依赖网络质量 |

---

## iOS 端跨服手册
 
- **iOS 端 → 安卓官服**：[点此跳转](/README_iOS2GW.md)

- **iOS 端 → Bilibili 服**：[点此跳转](/README_iOS2Bili.md)

- **iOS 端 → 渠道混服**：（结合以下“附录2”，参照跨 Bilibili 服教程操作）

---

## 附录1：App Store 链接

- **游戏本体**
  - 少女前线：<https://apps.apple.com/app/id1117273600>

- **网络调试工具（仅抓包）**
  - HTTP Catcher：<https://apps.apple.com/app/id1445874902>
  - iHTTP Tracker：<https://apps.apple.com/app/id1463315864>
  - Thor：<https://apps.apple.com/app/id1210562295>
- **网络调试工具（抓包、代理）**
  - Shadowrocket：<https://apps.apple.com/app/id932747118>
  - Quantumult X：<https://apps.apple.com/app/id1443988620>
  - Surge 4：<https://apps.apple.com/app/id1442620678>
  - Loon：<https://apps.apple.com/app/id1373567447>

## 附录2：「少女前线」国服客户端登录参数
 > 以下为分别连接不同的国服服务器时，有效的客户端登录参数。

### 官服

| 服务器 \ 参数 | URL / Host | Request Body<br/>`channel` | Request Body<br/>`device` | Request Body<br/>`platformChannelId` |
| :-: | :-: | :-: | :-: | :-: |
| 安卓官服 | ⋯`.gw.`⋯ | `cn_mica` | `adr` | `GWGW`<br/>`TapTap` |
| iOS 官服 | ⋯`.ios.`⋯ | `cn_appstore` | `ios` | `ios` |

### 渠道服

| 服务器 \ 参数 | URL / Host | Request Body<br/>`channel` | Request Body<br/>`device` | Request Body<br/>`platformChannelId` |
| :-: | :-: | :-: | :-: | :-: |
| Bilibili 服 | ⋯`.bili.`⋯ | `cn_bili` | `adr` | `Bili` |
| 渠道混服 | ⋯`.ly.`⋯ | `cn_third` | `adr` | `GWHF` |
