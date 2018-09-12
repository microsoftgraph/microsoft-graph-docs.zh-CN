# <a name="user-resource-type"></a>用户资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示 Azure Active Directory 用户对象。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出用户](../api/intune_shared_user_list.md) 对象。|[user](../resources/intune_shared_user.md) 集合|列出 [user](../resources/intune_shared_user.md) 对象的属性和关系。|
|[获取用户](../api/intune_shared_user_get.md) 对象。|[user](../resources/intune_shared_user.md) 集合|读取 [user](../resources/intune_shared_user.md) 对象的属性和关系。|
|[创建用户](../api/intune_shared_user_create.md)对象。|[user](../resources/intune_shared_user.md) 集合|创建新的 [user](../resources/intune_shared_user.md) 对象。|
|[删除用户](../api/intune_shared_user_delete.md) 。|无|删除 [user](../resources/intune_shared_user.md)。|
|[更新用户](../api/intune_shared_user_update.md)对象。|[用户](../resources/intune_shared_user.md)|更新 [user](../resources/intune_shared_user.md) 对象的属性。|
|**设备管理**|
|[removeAllDevicesFromManagement 操作](../api/intune_shared_user_removealldevicesfrommanagement.md)|无|停用该用户管理的所有设备|
|**移动应用程序管理 (MAM)**|
|[getManagedAppDiagnosticStatuses 函数](../api/intune_shared_user_getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) 集合|获取给定用户的诊断验证状态。|
|[getManagedAppPolicies 函数](../api/intune_shared_user_getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合|获取给定用户的应用限制。|
|[wipeManagedAppRegistrationsByDeviceTag 操作](../api/intune_shared_user_wipemanagedappregistrationsbydevicetag.md)|无|对含有指定设备标记的应用注册发布擦除操作。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|用户的唯一标识符。|
|**加入**|
|deviceEnrollmentLimit|Int32|允许用户注册的最大设备数的限制。 允许的值为 5 或 1000。|


## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**设备管理**|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md) 集合|与用户关联的管理设备。|
|**移动应用程序管理 (MAM)**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) 集合|属于用户的零个或多个托管的应用注册。|
|**疑难解答**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 集合|此用户的故障排除事件列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
