# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

自动更新模式可能的赋值。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|用户已定义，默认值，无特定意图。|
|notifyDownload|1|通知下载。|
|autoInstallAtMaintenanceTime|2|维护期间自动安装。|
|autoInstallAndRebootAtMaintenanceTime|3|维护期间自动安装和重新启动。|
|autoInstallAndRebootAtScheduledTime|4|在计划时间自动安装并重新启动。|
|autoInstallAndRebootWithoutEndUserControl|5|自动安装并重新启动，无需最终用户控制|








