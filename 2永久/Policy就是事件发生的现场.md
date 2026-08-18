---
type: permanent
created: "2026-08-18"
---
# Policy就是事件发生的现场

Policy可以继续调用的Command路由解耦其他业务逻辑，或者单独消费比如日志记录。
## 关联

- 依据：[[Reducer-Projection发生在Policy之前]]
- 产生：[[Command表示用户意图并不一定真正触发业务]]
- 上游：[[Event可作为业务事件发生的证据]]

## 来源

- 