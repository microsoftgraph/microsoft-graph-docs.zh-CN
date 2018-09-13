# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

管理代理类型。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|eas|1|设备由 Exchange Server 管理。|
|mdm|2|设备由 Intune MDM 管理。|
|easMdm|3|设备由 Exchange Server 和 Intune MDM 管理。|
|intuneClient|4|Intune 客户端托管。|
|easIntuneClient|5|设备是 EAS 和 Intune 客户端双重托管。|
|configurationManagerClient|8|设备由配置管理器托管。|
|configurationManagerClientMdm|10|设备由配置管理器和 MDM 托管。|
|configurationManagerClientMdmEas|11|设备由配置管理器、MDM 和 Eas 托管。|
|未知|16|未知的管理代理类型。|
|jamf|32|设备属性从 Jamf 获取。|
|googleCloudDevicePolicyController|64|设备由 Google 的 CloudDPC 托管。|








