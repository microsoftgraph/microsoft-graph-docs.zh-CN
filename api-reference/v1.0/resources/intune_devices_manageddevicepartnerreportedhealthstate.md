# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备健康状况 API 的可用健康状况
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|设备健康状况尚未报告|
|activated|1|移动威胁防御合作伙伴已激活设备，但尚未报告健康状况。|
|deactivated|2|移动威胁防御合作伙伴已停用设备。 设备健康状况未知。|
|secured|3|移动威胁防御合作伙伴认为设备安全。|
|lowSeverity|4|移动威胁防御合作伙伴认为设备威胁性低。|
|mediumSeverity|5|移动威胁防御合作伙伴认为设备威胁性中等。|
|highSeverity|6|移动威胁防御合作伙伴认为设备威胁性高。|
|unresponsive|7|移动威胁防御合作伙伴认为设备未响应。 设备健康状况未知。|
|compromised|8|设备被视为受到威胁防御合作伙伴破坏。 这意味着设备有一个无法由最终用户轻松修正的主动威胁或风险，因此用户应联系其 IT 管理员。|
|misconfigured|9|设备被认为与威胁防御伙伴配置错误。 这意味着设备缺少必需的配置文件或便威胁防御伙伴能够正常工作配置，因此威胁或风险分析无法完成。|








