# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

FirewallCertificateRevocationListCheckMethod 的可能值
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|配置通过 Intune，没有值不会替代的用户配置设备默认值|
|无|1|不检查证书吊销列表|
|尝试|2|尝试 CRL 检查并检查确认证书时才允许证书|
|需要|3|需要之前允许证书的 CRL 检查成功|



