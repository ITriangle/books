

## ZooKeeper 会话

ZooKeeper的API围绕ZooKeeper的句柄（ handle） 而构建， 每个API
调用都需要传递这个句柄。 这个句柄代表与ZooKeeper之间的一个会
话。


ZooKeeper服务器会在本地处理只读请求（ exists、 getData和
getChildren） 。 

LOOKING
LEADING
FOLLOWING


之后我们需要面对的问题便是服务器如何确认一个事务是否已经提
交， 由此引入了我们所采用的协议： Zab： ZooKeeper原子广播协议
（ ZooKeeper Atomic Broadcast protocol） 

