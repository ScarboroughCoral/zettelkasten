开启后preload的全局变量无法在加载页面中访问，反之亦然，只能通过contextBridge安全暴露。
## 关联

- 应用：[[contextBridge应当暴露有限制的方法而不是完全方法]]

## 来源

- [Context Isolation](https://www.electronjs.org/docs/latest/tutorial/context-isolation)
- [[Electron要对不可信来源进行隔离加载]]