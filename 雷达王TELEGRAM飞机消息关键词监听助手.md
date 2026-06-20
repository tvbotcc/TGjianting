# TGjianting
雷达王TELEGRAM飞机关键词监听助手 TG:@leidajianting
# 🛰️ 雷达王TELEGRAM飞机监听助手

> **多账号 Telegram 群组/频道监控 + 自动回复 + 自动加群一体化管理平台**

![C#](https://img.shields.io/badge/language-C%23-blue?logo=.net)
![.NET](https://img.shields.io/badge/.NET-10.0-512BD4?logo=dotnet)
![Docker](https://img.shields.io/badge/deploy-Docker-2496ED?logo=docker)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-lightgrey)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 📋 功能总览
### 📊 数据看板
- 可视化图表：消息趋势、关键词命中排行、账号活跃度
- 实时顶部状态栏：今日消息、总计消息、今日回复、加群成功数
- 全自动刷新
<img width="2117" height="1592" alt="image" src="https://github.com/user-attachments/assets/2d2825f2-d96d-4fad-bca0-aa151765af48" />

### 🔍 多账号消息监控
- 同时管理**多个 Telegram 账号**，每个账号独立登录、独立运行
- 实时监控指定群组/频道的消息流
- 支持24小时不间断监听，自动重连保活
- 监控/客服双角色账号分离
<img width="2062" height="827" alt="image" src="https://github.com/user-attachments/assets/4aa4b765-cca2-463e-91bb-b5e81bdf4ca1" />

### 🔑 关键词规则引擎
- 灵活的关键词匹配规则：包含、排除、正则表达式
- 支持按账号、按群组筛选匹配范围
- 排除规则优先级高于包含规则，精确控制触发条件
- 消息归档查询，可回溯历史匹配记录
<img width="2017" height="1182" alt="image" src="https://github.com/user-attachments/assets/bcb5cf62-ddbb-4d92-b760-72d8ed97e861" />

### 🤖 Bot 通知系统
- 关键词命中后通过 Bot 即时推送通知到指定群组/私聊
- 可自定义通知模板（HTML 格式）
- 支持 **Inline Keyboard** 一键跳转按钮
- 多级通知设置：指定命中后通知哪些 Bot、发往哪里
- 跨账号消息去重，避免重复通知
<img width="2062" height="862" alt="image" src="https://github.com/user-attachments/assets/7dacb591-ec8c-4f0a-90e0-ecc9778030e3" />

### 💬 自动回复
- 智能客服号池轮询回复，分摊消息压力
- 延迟随机化，模拟真人回复行为
- 多模板加权轮换，回复内容多样化
- 支持入库统计回复次数和发送时间
<img width="2075" height="946" alt="image" src="https://github.com/user-attachments/assets/faf85a97-561c-4325-871d-7f7b950721fc" />

### 🌐 Webhook 集成
- 关键词命中后回调指定 URL（POST JSON）
- 可自定义回调地址和开关控制
- 便于对接第三方系统
<img width="2062" height="707" alt="image" src="https://github.com/user-attachments/assets/2a6d729d-9961-4501-879f-e10aa9473b30" />

### ⏳ 自动加群管理
- **智能批次冷却系统**：5群→5分 / 6群→8分 / 5群→10分 循环
- 支持并发加群，可自定义并发数（1-10）
- 每日/每小时加群上限控制
- FLOOD_WAIT 自动检测与冷却
- 无效链接自动跳过并尝试备用模式（邀请链接 ↔ 公开群链接自动切换）
- 失败自动重试 + 超时保护（90秒）
- 实时状态面板：查看每个账号的当前操作、批次进度、冷却剩余时间
- 手动/自动双模式
<img width="2095" height="1817" alt="image" src="https://github.com/user-attachments/assets/e1dba6fc-42b0-41c8-9448-348ff7fdbcbb" />

### 🔄 代理池
- 多订阅源管理（支持 Clash/Mihomo/V2Ray 等格式）
- 自动解析 YAML/Base64 订阅
- TCP 延迟测试，自动排序优选节点
- 按账号独立分配代理
- 定时自动刷新订阅
<img width="2052" height="1236" alt="image" src="https://github.com/user-attachments/assets/28824624-f55b-4d60-b1df-05ace017d5fc" />

### 🔐 登录保护
- 每账号独立登录保护开关
- 删除/断连操作二次确认
- Session 自动持久化，重启无需重新登录



### ⚙ 系统管理
- 一键暂停/恢复全部监控
- 消息自动清理（可配置保留时长）
- 数据库备份与恢复
- API 设置（Bot Token、Admin ID 等）
- 深色/浅色主题切换



## 📖 使用教程

### 1️⃣ 添加账号
进入「账户管理」→ 添加手机号 → 输入验证码登录（支持 2FA）
> 账号分为 **监控号**（用于监听消息）和 **客服号**（用于自动回复）

### 2️⃣ 设置关键词规则
进入「关键词规则」→ 添加关键词 → 设置匹配范围和通知 Bot
> 支持设置排除规则和监控全局消息

### 3️⃣ 配置 Bot 通知
进入「Bot 通知」→ 添加 Bot Token → 配置通知目标群组
> 支持自定义消息模板和 Inline 跳转按钮

### 4️⃣ 开始监控
进入「数据看板」→ 点击顶部状态栏查看实时数据
> 系统自动运行，无需手动干预



**雷达王TELEGRAM飞机监听助手**

咨询 TG：@leidajianting

---

> ⚠️ **免责声明**：本工具仅供学习和研究使用，请遵守 Telegram 服务条款及当地法律法规。
> google-site-verification: google3f87f39ce7b3e4b6.html
