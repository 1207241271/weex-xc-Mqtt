# weex-xc-Mqtt

#### 一款Mqtt weex插件




#####  connect(String host,int port,func callback)
+ 连接至MQTT
+ callback参数

| 属性       		| 类型	     	| 示例		  | 描述              |
| ------------- 	|:---------:	| -----:	  | ----------:      |
|suc		|bool		|true	  | 是否成功|


#####  setMqttReceiver(fuc callback)
+ 设置MQTT消息接收

| 属性       		| 类型	     	| 示例		  | 描述              |
| ------------- 	|:---------:	| -----:	  | ----------:      |
|topic		|String		|dev2app/865067022403441/433	  | 发出消息的topic|
|data		|Object		| {"code":0,"data":{}}  | 解析出的返回数据      |



#####  subscribe(String topic,fuc callback)
+ 订阅主题topic 

#####  subscribeTopics(Array topics,func callback)
+ 订阅主题topics 

#####  unSubscribe(String topic,func callback)
+ 解除订阅topic

#####  unSubscribeTopics(Array topics,func callback)
+ 解除订阅topics

##### publish(String topic,Object data)
+ 发送消息

##### disconnect(func callback)
+ 关闭连接

#### 使用Jpush模块

``` html 
<script>
  const Mqtt = weex.requireModule('Mqtt');
  module.exports = {
    data: {
      
    },
    
    methods: {
	    subscribe() {
			Mqtt.connect(host,port,res=>{});
		}
	}
  };
</script>
```
