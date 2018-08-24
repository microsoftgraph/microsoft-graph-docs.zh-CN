# <a name="firewallpacketqueueingmethodtype-enum-type"></a>firewallPacketQueueingMethodType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

FirewallPacketQueueingMethod 的可能值
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|没有由 Intune 配置的值，不要替代用户配置的设备默认值|
|disabled|1|禁用数据包的队列|
|queueInbound|2|队列入站加密数据包|
|queueOutbound|3|队列解密出站数据包以进行转发|
|queueBoth|4|队列入站和出站数据包|



