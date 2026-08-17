---
type: permanent
created: "2026-08-17"
---
# contextBridge应当暴露有限制的方法而不是完全方法

contextBridge应当避免将类似`ipcRenderer.send`直接暴露出去，这样加载页面可能利用漏洞访问主进程node环境。
## 关联

- 支持：

## 来源

- [Security considerations](https://www.electronjs.org/docs/latest/tutorial/context-isolation#security-considerations)