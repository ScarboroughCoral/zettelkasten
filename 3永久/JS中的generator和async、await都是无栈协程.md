
有栈协程允许在普通嵌套函数中暂停协程，并在恢复后继续。

比如如下例子，`outer`是普通函数，无法暂停直接输出111没有停在`inner()`的调用位置，说明一定是无栈协程。
```typescript
function outer(){
	inner();
	console.log(111)
}
async function inner(){
	return await SomeTaskPromise()
}
```
## 关联

- 支持：[[协程是可暂停、存储暂停状态、可恢复的程序单元]]

## 来源

- 