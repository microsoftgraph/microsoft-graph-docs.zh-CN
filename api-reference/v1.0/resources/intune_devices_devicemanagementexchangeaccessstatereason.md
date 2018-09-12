# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备 Exchange 访问状态的原因。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|none|0|没有从 Exchange 中发现访问状态的原因|
|unknown|1|未知的访问状态的原因|
|exchangeGlobalRule|2|访问状态由 Exchange 全局规则确定|
|exchangeIndividualRule|3|访问状态由 Exchange 单个规则确定|
|exchangeDeviceRule|4|访问状态由 Exchange 设备规则确定|
|exchangeUpgrade|5|访问状态取决于 Exchange 升级|
|exchangeMailboxPolicy|6|访问状态由 Exchange 邮箱策略确定|
|other|7|访问状态由 Exchange 确定|
|compliant|8|访问状态由合规性质询授权|
|notCompliant|9|访问状态由合规性质询吊销|
|notEnrolled|10|访问状态由管理质询吊销|
|unknownLocation|12|未知位置的访问状态|
|mfaRequired|13|MFA 质询的访问状态|
|azureADBlockDueToAccessPolicy|14|访问状态由 AAD 访问策略吊销|
|compromisedPassword|15|访问状态由泄露的密码吊销|
|deviceNotKnownWithManagedApp|16|访问状态由托管应用程序质询吊销|








