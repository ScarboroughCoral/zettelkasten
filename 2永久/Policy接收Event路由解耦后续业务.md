---
type: permanent
created: "2026-08-18"
---
# Policy接收Event路由解耦后续业务

Policy就是事件发生的现场，可以调用的Command，或者单独消费比如日志记录。
## 关联

- 产生：[[Command表示用户意图并不一定真正触发业务]]
- 上游：[[Event可作为业务事件发生的证据]]
- 依据：[[Reducer-Projection发生在Policy之前]]

## 来源

- 