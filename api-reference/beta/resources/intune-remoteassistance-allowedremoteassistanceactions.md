---
title： "allowedRemoteAssistanceActions enum type" description： "Flags enumeration indicating whether a helper can establish a "View screen"， "Take full control" and "Elevation" remote assistance action with a device or sharer" author： "dougeby" localization_priority： Normal ms.prod： "intune" doc_type： enumPageType
---

# <a name="allowedremoteassistanceactions-enum-type"></a>allowedRemoteAssistanceActions 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Flags 枚举，指示帮助程序是否可以与设备或共享者建立"查看屏幕"、"完全控制"和"提升"远程协助操作

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|viewScreen|1|帮助程序可以查看共享者设备的屏幕|
|takeFullControl|2|帮助程序可以完全控制共享者的设备|
|elevation|4 |帮助程序可以使用提升的权限完全控制共享者的设备|



