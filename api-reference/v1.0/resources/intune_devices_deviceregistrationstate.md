# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备注册状态。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notRegistered|0|未注册设备。|
|registered|2|已注册设备。|
|revoked|3|已阻止、擦除或停用该设备。|
|keyConflict|4|设备存在重大冲突。|
|approvalPending|5|设备处于待审批状态。|
|certificateReset|6|设备证书已被重置。|
|notRegisteredPendingEnrollment|7|未注册设备以及待处理注册。|
|unknown|8|设备注册状态未知。|



