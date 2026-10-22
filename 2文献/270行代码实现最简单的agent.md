## 作者的主张

最少代码实现一个claudecode，包含tools 和api call。
答题思路，从外层到内层：
1. 最外层处理用户输入，是退出、用户输入还是其他
2. 如果是用户输入则进入agent loop层
3. 将用户的输入加到历史messages数组里请求大模型包含tools数组、用户messages上下文
	1. tools包含描述、参数协议
4. 大模型返回tools

## 来源信息

https://github.com/1rgs/nanocode/blob/master/nanocode.py