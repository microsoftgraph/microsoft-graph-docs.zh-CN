# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

firewallCertificateRevocationListCheckMethod 可能的值
## <a name="members"></a>成员
|成员|值|描述|
|:---|:---|:---|
|deviceDefault|0|没有由 Intune 配置的值，不要替代用户配置的设备默认值|
|无|1|不检查证书吊销列表|
|尝试|2|尝试 CRL 检查并且检查确认证书后才允许使用证书|
|需要|3|允许使用证书之前需要 CRL 检查成功|



