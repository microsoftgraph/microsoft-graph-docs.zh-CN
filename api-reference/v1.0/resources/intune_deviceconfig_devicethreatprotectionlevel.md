# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备威胁保护 API 的设备威胁保护级别。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unavailable|0|默认值。 请勿使用。|
|secured|1|设备威胁级别要求：安全。 这是最安全的级别，表示在设备上未发现任何威胁。|
|low|2|设备威胁保护级别要求：低。 低代表会为设备或设备数据带来小量风险的威胁严重性。|
|medium|3|设备威胁保护级别要求：中等。 中等代表为设备或设备数据带来中等风险的威胁严重性。|
|high|4|设备威胁保护级别要求：高。 高代表会为设备或设备数据造成严重风险的威胁严重性。|
|notSet|10|设备威胁保护级别要求：未设置。 未设置表示设备不要求满足特定威胁保护级别。|








