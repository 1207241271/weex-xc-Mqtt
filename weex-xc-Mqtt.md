# weex-xc-Mqtt

#### 一款Mqtt weex插件


#####  connect(String host,int port,func callback)
+ 连接至MQTT

#####  setMqttReceiver(fuc callback)
+ 设置MQTT消息接收

#####  subscribe(String topic,fuc callback)
+ 订阅主题topic 

#####  subscribeTopics(Array topics,func callback)
+ 订阅主题topics 

#####  unSubscribe(String topic,func callback)
+ 解除订阅topic

#####  unSubscribe(Array topics,func callback)
+ 解除订阅topics

##### publish(String topic,Object data)
+ 发送消息


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
