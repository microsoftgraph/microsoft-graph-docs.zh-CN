# <a name="device-resource-type"></a>设备资源类型

表示在组织中注册的设备。也可以在云中使用设备注册服务或通过 Intune 创建设备。条件访问策略使用它们进行多重身份验证。这些设备范围很广，从台式机、笔记本电脑到手机和平板电脑均包括在内。继承自 [directoryObject](directoryobject.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建设备](../api/device_post_devices.md) | [设备](device.md) |在目录中新建注册设备。|
|[获取设备](../api/device_get.md) | [设备](device.md) |读取 device 对象的属性和关系。|
|[列出设备](../api/device_list.md) | [设备](device.md) 集合| 检索目录中的注册设备列表。 |
|[更新设备](../api/device_update.md) | [设备](device.md) |更新 device 对象的属性。 |
|[删除设备](../api/device_delete.md) | 无 |删除 device 对象。 |
|[创建 registeredOwner](../api/device_post_registeredowners.md) |[directoryObject](directoryobject.md)| 通过发布到 registeredOwners 导航属性，将用户添加为该设备的新所有者。|
|[列出 registeredOwners](../api/device_list_registeredowners.md) |[directoryObject](directoryobject.md) 集合| 从 registeredOwners 导航属性中获取身份为设备的注册所有者的用户。|
|[创建 registeredUser](../api/device_post_registeredusers.md) |[directoryObject](directoryobject.md)| 通过发布到 registeredUsers 导航属性，为该设备添加新注册用户。|
|[列出 registeredUsers](../api/device_list_registeredusers.md) |[directoryObject](directoryobject.md) 集合| 从 registeredUsers 导航属性获取设备的注册用户。|

## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| 启用帐户时为 **true**，否则为 **false**。必需。|
|alternativeSecurityIds|[alternativeSecurityId](alternativesecurityid.md) 集合| 需要多值属性筛选器表达式的**任意**运算符。不可为 NULL。必需。 |
|approximateLastSignInDateTime|DateTimeOffset| 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|deviceId|Guid| 唯一客户端指定 GUID 以表示该设备。必需。 |
|deviceMetadata|String|    |
|deviceVersion|Int32|            |
|displayName|String|设备显示名称。必需。 |
|id|String|设备唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL。只读。|
|isCompliant|Boolean|如果设备符合移动设备管理 (MDM) 策略，则为 **true**，否则为 **false**。|
|isManaged|Boolean|如果用移动设备管理 (MDM) 应用（例如 Intune）管理设备，则为 **true**，否则为 **false**。|
|onPremisesLastSyncDateTime|DateTimeOffset|对象最后一次与本地目录同步的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|onPremisesSyncEnabled|Boolean|如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **NULL**（默认值）。|
|operatingSystem|String|设备上操作系统的类型。必需。 |
|operatingSystemVersion|String|设备上操作系统的版本。必需。 |
|physicalIds|String collection| 不可为 NULL。            |
|trustType|String|    ||

## <a name="relationships"></a>关系
| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|registeredOwners|[directoryObject](directoryobject.md) 集合|是设备注册所有者的用户。只读。可为 NULL。|
|registeredUsers|[directoryObject](directoryobject.md) 集合|身份为设备注册用户的用户。只读。可为 NULL。|



## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "alternativeSecurityIds": [{"@odata.type": "microsoft.graph.alternativeSecurityId"}],
  "approximateLastSignInDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "trustType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
