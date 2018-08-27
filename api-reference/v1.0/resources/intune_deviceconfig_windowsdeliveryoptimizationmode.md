# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

节点分发的传递优化模式
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|httpOnly|1|仅HTTP ，无对等互联|
|httpWithPeeringNat|2|OS 默认 – Http 与同一网络地址转换器后进行对等互联混合|
|httpWithPeeringPrivateGroup|3|HTTP 与跨专用组对等互联混合|
|httpWithInternetPeering|4|HTTP 与 Internet 对等互联混合|
|simpleDownload|99|无对等互联的简单下载模式|
|bypassMode|100|旁路模式。 不要使用传递优化，而应使用BITS|



