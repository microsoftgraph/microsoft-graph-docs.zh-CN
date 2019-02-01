---
title: 设备资源类型
description: 表示在组织中注册的设备。 可以在云中使用设备注册服务或 Intune 创建设备。 条件访问策略使用它们进行多重身份验证。 这些设备范围很广，从台式机、笔记本电脑到手机和平板电脑均包括在内。 继承自 directoryObject。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9b69f51e045bff43d4c250f2b00791000df1499e
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2019
ms.locfileid: "29690922"
---
# <a name="device-resource-type"></a>设备资源类型

表示在组织中注册的设备。 可以在云中使用设备注册服务或 Intune 创建设备。 条件访问策略使用它们进行多重身份验证。 这些设备范围很广，从台式机、笔记本电脑到手机和平板电脑均包括在内。 继承自 [directoryObject](directoryobject.md)。

使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取设备](../api/device-get.md) | [设备](device.md) |读取 device 对象的属性和关系。|
|[列出设备](../api/device-list.md) | [设备](device.md) 集合| 检索目录中的注册设备列表。 |
|[更新设备](../api/device-update.md) | [设备](device.md) |更新 device 对象的属性。 |
|[删除设备](../api/device-delete.md) | 无 |删除 device 对象。 |
|[List memberOf](../api/device-list-memberof.md) |[directoryObject](directoryobject.md) collection| 列出设备位于直接成员的组。 |
|[列出 registeredOwners](../api/device-list-registeredowners.md) |[directoryObject](directoryobject.md) collection| 通过 registeredOwners 导航属性，获取身份为设备注册所有者的用户。|
|[列出 registeredUsers](../api/device-list-registeredusers.md) |[directoryObject](directoryobject.md) 集合| 从 registeredUsers 导航属性获取设备的注册用户。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| 启用帐户时为 **true**，否则为 **false**。必需。|
|alternativeSecurityIds|alternativeSecurityId 集合| 仅供内部使用。 不可为 null。 |
|approximateLastSignInDateTime|DateTimeOffset| 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：`'2014-01-01T00:00:00Z'`。只读。 |
|deviceId|string| 由 Azure 设备注册服务在设备注册时设置的唯一标识符。 |
|deviceMetadata|String| 仅供内部使用。 设置为 null。 |
|deviceVersion|Int32| 仅供内部使用。 |
|displayName|String|设备显示名称。必需。 |
|id|字符串|设备唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL。只读。|
|isCompliant|Boolean|如果设备符合移动设备管理 (MDM) 策略，则为 **true**；否则；为 **false**。 只读。 此值只可以由 Intune 的任何设备操作系统类型或[批准 MDM 应用程序](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)的 Windows 操作系统设备更新。|
|isManaged|Boolean|如果设备由移动设备管理 (MDM) 应用进行托管，则为 **true**；否则，为 **false**。 此值只可以由 Intune 的任何设备操作系统类型或[批准 MDM 应用程序](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)的 Windows 操作系统设备更新。 |
|onPremisesLastSyncDateTime|DateTimeOffset|对象最后一次与本地目录同步的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|onPremisesSyncEnabled|Boolean|如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。 只读。 |
|operatingSystem|String| 设备上操作系统的类型。必需。 |
|operatingSystemVersion|String|设备上操作系统的版本。必需。 |
|physicalIds|String 集合| 仅供内部使用。 不可为 null。 |
|trustType|String| 加入设备的信任类型。 只读。 可取值为： <br />**Workplace** - 表示*自带个人设备*<br />**AzureAd** - 仅云加入设备<br />**ServerAd** - 加入 Azure AD 的本地域加入设备。 如需了解更多详情，请参阅 [Azure Active Directory 中的设备管理简介](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|extensions|[扩展](extension.md)集合|为设备定义的开放扩展集合。只读。可为 NULL。|
|memberOf|[directoryObject](directoryobject.md) collection|此组所属的组。HTTP 方法：GET（支持所有组）只读。可为 Null。|
|[List transitive memberOf](../api/device-list-transitivememberof.md) |[directoryObject](directoryobject.md) 集合| 列出的组的成员的设备。 此操作是传递的。 |
|registeredOwners|[directoryObject](directoryobject.md) collection|云加入设备或已注册个人设备的用户。 已注册的所有者是在注册时设置。 目前，只能有一个所有者。 只读。 可为 Null。 |
|registeredUsers|[directoryObject](directoryobject.md) 集合|设备的已注册用户集合。 对于云加入设备和已注册的个人设备，已注册用户在设备注册时设置为与已注册所有者相同的值。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
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

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
