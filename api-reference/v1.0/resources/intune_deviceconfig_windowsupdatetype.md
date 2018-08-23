# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

将从哪些分支设备接收其更新
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|所有|1|半年频道（定向）。 设备从半年频道（定向）中获取所有适用的功能更新。|
|businessReadyOnly|2|半年频道。 设备从半年频道获取功能更新。|
|windowsInsiderBuildFast|3|Windows 预览体验内部版本 - 快|
|windowsInsiderBuildSlow|4|Windows 预览体验内部版本 - 慢|
|windowsInsiderBuildRelease|5|发布 Windows 预览体验内部版本|



