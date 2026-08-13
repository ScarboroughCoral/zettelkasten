---
type: source
created: 2026-08-13
---

# Electron 要对不可信来源进行隔离处理

## 作者的观点
永远不要对不可信来源开启nodeIntegration = true，使用webview、WebContentView隔离加载页面，禁用node集成，开启contextIsolation。
## 我的理解
不可信来源比如远端服务器的代码能够随意写代码来访问用户本地的数据，操作文件系统，访问网络，执行非法程序，这是不安全的。不使用contextIsolation就会放宽非法状态的可能性。
## 来源信息
- 页码或网址：https://www.electronjs.org/docs/latest/tutorial/security#isolation-for-untrusted-content
- 查阅日期：2026-08-13