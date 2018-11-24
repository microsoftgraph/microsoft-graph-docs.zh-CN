# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

AppLocker 应用程序控件类型的可能值
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，未选择的应用程序控制类型。|
|enforceComponentsAndStoreApps|1|强制实施 Windows 组件和 store 应用程序。|
|auditComponentsAndStoreApps|2|审核 Windows 组件和 store 应用程序。|
|enforceComponentsStoreAppsAndSmartlocker|3|强制实施 Windows 组件、 存储应用程序和智能锁定者。|
|auditComponentsStoreAppsAndSmartlocker|4|审核 Windows 组件，存储应用程序和智能锁定者。|



