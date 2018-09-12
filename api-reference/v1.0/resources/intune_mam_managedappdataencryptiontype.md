# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代表向其应用程序数据进行加密托管的应用程序级别
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useDeviceSettings|0|应用程序数据根据设备默认设置进行加密。|
|afterDeviceRestart|1|应用程序数据在设备重新启动时进行加密。|
|whenDeviceLockedExceptOpenFiles|2|与此策略关联的应用程序数据在设备锁定时进行加密，文件中打开的数据除外|
|whenDeviceLocked|3|与此策略关联的应用程序数据在设备锁定时进行加密|








