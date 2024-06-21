使用步骤
1.开启mqserver
2.编译：
go build product.go
go build consume1.go
go build consume2.go

3.运行
./consume1 1   //表示队列绑定路由key1
./consume2 2   //表示队列绑定路由key2
./product 1   //表示给路由key = 1 发消息


#多次执行./product 1  发现consume1 ，consume2 都会接受到消息！！！

