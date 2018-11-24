# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

对等方通讯组的传递优化模式
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|允许用户设置。|
|为 httpOnly|1|HTTP 仅，没有对等|
|httpWithPeeringNat|2|与同一个网络地址转换器后面对等的 OS 默认 – Http 混合|
|httpWithPeeringPrivateGroup|3|HTTP 与跨专用组对等混合|
|httpWithInternetPeering|4|与 Internet 对等混合的 HTTP|
|simpleDownload|99|与没有对等的简单 download 模式|
|bypassMode|100|绕过模式。 不使用传递优化并改用位|



