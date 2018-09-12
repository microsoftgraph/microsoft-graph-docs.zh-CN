# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

允许该设备发送诊断和使用情况的遥测数据，如 Watson。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|none|1|从操作系统组件不发送任何遥测数据。 注意：此值仅适用于企业和服务器设备。 在其他设备上使用此设置等效于将值设为 1。|
|basic|2|发送基本遥测数据。|
|enhanced|3|发送包括使用情况和见解数据的增强型遥测数据。|
|full|4|发送全 部遥测数据，包括诊断数据（如系统状态）。|








