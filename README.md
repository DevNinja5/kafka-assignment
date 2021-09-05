## Producer

### To produce a single line message
Add your message in ProducerRecord
```java
ProducerRecord<String,String> record = new ProducerRecord<>("mytopic2","Hope this is running well");
```
Here `mytopic2` is name of ***topic*** and `Hope this is running well` is ***message***.

## Consumer
### To see consuming messages
Make sure you subscribed to the topic `mytopic2`
```java
String topic="mytopic2";
consumer.subscribe(Arrays.asList(topic));
```
### Then
Just run the `Consumer.java` file. A terminal will open and there you can see your all messages from beginning produced by Producer.
