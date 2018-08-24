# <a name="compliancestate-enum-type"></a>complianceState 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

合规性状态。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知。|
|compliant|1|合规。|
|noncompliant|2|设备不合规，并阻止访问企业资源。|
|conflict|3|与其他规则冲突。|
|error|4|错误。|
|inGracePeriod|254|设备不合规，但仍有权访问公司资源|
|configManager|255|由配置管理器管理|



