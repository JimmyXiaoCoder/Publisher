# Publisher
mq学习demo(rabbitmq)

笔记：
    交换机<br>
    队列<br>
    路由<br>
    上述三者需绑定一起才算完成了消息发送者的配置<br>
    直连交换机：<br>
        一个交换机只能绑定一个队列一个路由<br>
    主题交换机：<br>
        一个交换机可以绑定多个路由，多个队列<br>
    扇形交换机：<br>
        一个交换机可以绑定多个队列，并将交换机获取的消息发送给所有绑定的队列中<br>
    区别：<br>
        虽说主题交换机可以实现类似扇形路由器的功能，但是两者对于消息收发的控制精度有区别，扇形交换机会将消息发送给所有绑定到交换机的队列，类似广播的效果，而主题交换机由于有要设置路由的存在，所以消息的发送范围大概率没有扇形那么广<br>