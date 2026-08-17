---
type: source
created: "2026-08-13"
---
# Electron要对不可信来源进行隔离加载

## 作者的主张

永远不要对不可信来源开启nodeIntegration = true，使用webview、WebContentView隔离加载页面，禁用node集成，开启contextIsolation。

## 来源信息

网址：[Isolation for untrusted content](https://www.electronjs.org/docs/latest/tutorial/security#isolation-for-untrusted-content)

## 值得继续思考的问题

- 是否需要验证？
- 是否可能产生永久笔记？
- [[contextIsolation具体在哪里起作用]]