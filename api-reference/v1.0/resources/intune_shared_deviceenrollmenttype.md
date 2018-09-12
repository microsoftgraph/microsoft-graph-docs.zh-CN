# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

将移动设备添加到管理的可能方式。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值，未收集注册类型。|
|userEnrollment|1|通过 BYOD 通道完成用户驱动的注册。|
|deviceEnrollmentManager|2|使用设备注册管理器帐户完成用户注册。|
|appleBulkWithUser|3|Apple 批量注册，但用户可以质询（DEP、Apple 配置器）。|
|appleBulkWithoutUser|4|Apple 批量注册，但用户不可质询。（DEP、Apple 配置器、Mobile 配置）。|
|windowsAzureADJoin|5|Windows 10 Azure AD Join|
|windowsBulkUserless|6|通过 ICD 完成 Windows 10 批量注册，并提供证书。|
|windowsAutoEnrollment|7|Windows 10 自动注册。 （添加单位帐户）|
|windowsBulkAzureDomainJoin|8|Windows 10 bulk Azure AD Join。|
|windowsCoManagement|9|Windows 10 共同管理通过 AutoPilot 或组策略触发。|



