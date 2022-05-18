---
title: 设备资源类型
description: 表示在目录中注册的设备。
ms.localizationpriority: medium
author: sandeo-MSFT
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f8233f2f54a49fbe02f5cb5d51ad5250dbf7fff
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461563"
---
# <a name="device-resource-type"></a>设备资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在目录中注册的设备。 可以在云中使用设备注册服务或 Intune 创建设备。 条件访问策略使用它们进行多重身份验证。 这些设备范围很广，从台式机、笔记本电脑到手机和平板电脑均包括在内。 继承自 [directoryObject](directoryobject.md)。

使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。 此资源是允许传入其他属性的开放类型。

## <a name="methods"></a>Methods

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取设备](../api/device-get.md) | [设备](device.md) |读取设备对象的属性和关系。|
|[列出设备](../api/device-list.md) | [设备](device.md) 集合| 检索目录中的注册设备列表。 |
|[更新设备](../api/device-update.md) | [设备](device.md)  |更新设备对象的属性。 |
|[删除设备](../api/device-delete.md) | 无 |删除设备对象。 |
|[List memberOf](../api/device-list-memberof.md) |[directoryObject](directoryobject.md) collection| 列出设备是其直接成员的组和管理单元。 |
|[List transitive memberOf](../api/device-list-transitivememberof.md) |[directoryObject](directoryobject.md) 集合| 列出设备所属的组和管理单元。 此操作是可传递的。 |
|[列出 registeredOwners](../api/device-list-registeredowners.md) |[directoryObject](directoryobject.md) 集合| 通过 registeredOwners 导航属性，获取身份为设备注册所有者的用户。|
|[列出 registeredUsers](../api/device-list-registeredusers.md) |[directoryObject](directoryobject.md) 集合| 从 registeredUsers 导航属性获取设备的注册用户。|
|[列表 usageRights](../api/device-list-usagerights.md) | [usageRight](usageright.md) 集合 | 获取授予设备的使用权限的集合。|
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md) | String collection | 检查组列表中的成员身份。检查是可传递的。 |
| [getMemberGroups](../api/directoryobject-getmembergroups.md) | String collection | 返回设备所属的所有组。 检查是可传递的。 |
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md) | String 集合 | 检查组、目录角色或管理单元对象列表中的成员身份。 |
|[getMemberObjects](../api/directoryobject-checkmemberobjects.md) | String collection | 返回设备所属的所有组、管理单元和目录角色。 检查是可传递的。 |
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|

## <a name="properties"></a>属性

> [!IMPORTANT]
> 仅当使用设置为 `eventual` 和 `$count` 的 **ConsistencyLevel** 标头时，才支持 `$filter` 和 `$search` 查询参数的特定用法。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries#device-properties)。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| 启用帐户时为 `true`，否则为 `false`。 默认值为“`true`”。 <br/><br/> 支持 `$filter`（`eq`、`ne`、`not`、`in`）。 只有全局管理员和云设备管理员角色中的调用方才能设置此属性。|
|alternativeSecurityIds|[alternativeSecurityId](alternativeSecurityId.md) 集合| 仅供内部使用。 不可为 null。 支持 `$filter`（`eq`、`not`、`ge`、`le`）。 |
|approximateLastSignInDateTime|DateTimeOffset| 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 支持`$filter` (`eq`、`ne`、`not`、`ge``le`和`eq`值`null`) 和 `$orderBy`。 |
|complianceExpirationDateTime|DateTimeOffset| 设备不再被视为符合时的时间戳。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
|deviceCategory|String|用户定义的属性由Intune设置为自动将设备添加到组并简化设备管理。|
|deviceId|String| 注册时由 Azure 设备注册服务设置的标识符。 支持 `$filter`（`eq`、`ne`、`not`、`startsWith`）。 |
|deviceMetadata|String| 仅供内部使用。 设置为 `null`。 |
|deviceOwnership|String|设备的所有权。 此属性由Intune设置。 可取值为：`unknown`、`company`、`personal`。|
|deviceVersion|Int32| 仅供内部使用。 |
|displayName|String| 设备显示名称。 必需。 支持 `$filter` (`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`)、`$search` 和 `$orderBy`。  |
|domainName|String|已加入混合 Azure AD 的设备的本地域名。 此属性由Intune设置。|
|enrollmentProfileName|字符串|应用到设备的注册配置文件。 例如，`Apple Device Enrollment Profile``Device enrollment - Corporate device identifiers`或 `Windows Autopilot profile name`. 此属性由Intune设置。|
|enrollmentType|String|设备的注册类型。 此属性由Intune设置。 可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。|
| extensionAttributes | [onPremisesExtensionAttributes](onpremisesextensionattributes.md) | 包含设备的扩展属性 1-15。 不能选择单个扩展属性。 这些属性在云中掌握，可以在 Azure AD 中创建或更新设备对象期间进行设置。 <br><br>支持 `$filter`（`eq`、`not`、`startsWith` 和 `null` 值上的 `eq`）。|
|id|String|设备唯一标识符。 继承自 [directoryObject](directoryobject.md)。 密钥，不可为 NULL。 只读。 支持 `$filter` （`eq`、 `ne`、 `not`、 `in`）。 |
|isCompliant|Boolean|`true`如果设备符合移动设备管理 (MDM) 策略，则为 ɭ;否则为 `false`。 只读。 这只能通过任何设备 OS 类型的Intune或Windows OS 设备的[已批准 MDM 应用](/windows/client-management/mdm/azure-active-directory-integration-with-mdm)进行更新。 支持 `$filter`（`eq`、`ne`、`not`）。|
|isManaged|Boolean|`true`如果设备由移动设备管理 (MDM) 应用管理，则为 ！;否则为 `false`。 这只能通过任何设备 OS 类型的Intune或Windows OS 设备的[已批准 MDM 应用](/windows/client-management/mdm/azure-active-directory-integration-with-mdm)进行更新。 支持 `$filter`（`eq`、`ne`、`not`）。 |
|isRooted|布尔值|`true` 如果设备处于根基状态; `false` 如果设备已越狱， 这只能通过Intune进行更新。|
|managementType|String|设备的管理通道。  此属性由Intune设置。 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。|
|manufacturer|String| 设备制造商。 只读。 |
|mdmAppId|String|用于将设备注册到 MDM 的应用程序标识符。 只读。 支持 `$filter` （`eq`、 `ne`、 `not`、 `startsWith`）。|
|model|String| 设备的模型。 只读。 |
|onPremisesLastSyncDateTime|DateTimeOffset|上次将对象与本地目录同步的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 是 `2014-01-01T00:00:00Z` 只读的。 支持 `$filter` （`eq`、 `ne`、 `not`、 `ge`、 `le`、 `in`）。 |
|onPremisesSyncEnabled|Boolean|如果此对象从本地目录同步，则为 `true`；如果此对象最初从本地目录同步，但以后不再同步，则为 `false`；如果此对象从未从本地目录同步，则为 `null`（默认值）。 只读。 支持 `$filter`（`eq`、`ne`、`not`、`in` 和 `null` 值上的 `eq`）。 |
|operatingSystem|String| 设备上操作系统的类型。 必需。 支持`$filter` (`eq`、`ne`、`not`、`ge``le`和`startsWith``eq`值`null`) 。 |
|operatingSystemVersion|String| 设备的操作系统版本。 必填。 支持`$filter` (`eq`、`ne`、`not`、`ge``le`和`startsWith``eq`值`null`) 。 |
|physicalIds|String collection| 仅供内部使用。 不可为 null。 支持`$filter` (`eq`、`not`、`ge`和`le``startsWith`计数空集合) 。 |
|profileType|String|设备的配置文件类型。 可能的值： `RegisteredDevice` (默认) 、`SecureVM`、 `Printer`、 `Shared``IoT`|
|registrationDateTime|DateTimeOffset|设备注册的日期和时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|systemLabels|String collection| 系统应用于设备的标签列表。 在) `eq`计算空集合时支持`$filter` (。 |
|主机 名|String collection| 设备的 hostNames 列表。|
|trustType|String| 加入设备的信任类型。 只读。 可能的值： `Workplace` (指示 *将自己的个人设备)* ， `AzureAd` (仅加入云的设备) ， `ServerAd` (已加入 Azure AD) 的本地域设备。 如需了解更多详情，请参阅 [Azure Active Directory 中的设备管理简介](/azure/active-directory/device-management-introduction) |
|name| String | 设备的友好名称。 仅当用户在罗马Project使用 Microsoft 帐户登录时才返回。 |
|status | String| 设备是 `online` 或 `offline`. 仅当用户在罗马Project使用 Microsoft 帐户登录时才返回。 |
|平台 |String|设备平台。 仅当用户在罗马Project使用 Microsoft 帐户登录时才返回。 仅当用户在罗马Project使用 Microsoft 帐户登录时才返回。|
|kind| String| 设备的外形因子。 仅当用户在罗马Project使用 Microsoft 帐户登录时才返回。 |
|model| String| 设备模型。 仅当用户在罗马Project使用 Microsoft 帐户登录时才返回。 |
|manufacturer| String| 设备制造商。 仅当用户在罗马Project使用 Microsoft 帐户登录时才返回。 |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| 命令 | [命令](command.md) 集合 | 发送到此设备的命令集。|
|extensions|[扩展](extension.md)集合|为设备定义的开放扩展集合。只读。可为 NULL。 |
|memberOf|[directoryObject](directoryobject.md) 集合|此设备所属的组和管理单元。 只读。 可为 NULL。 支持 `$expand`。 |
|registeredOwners|[directoryObject](directoryobject.md) 集合| 云加入设备或已注册个人设备的用户。 已注册的所有者是在注册时设置。 目前，只能有一个所有者。 只读。 可为 NULL。 支持 `$expand`。 |
|registeredUsers|[directoryObject](directoryobject.md) 集合| 设备的已注册用户集合。 对于云加入设备和已注册的个人设备，已注册用户在设备注册时设置为与已注册所有者相同的值。 只读。 可为 NULL。 支持 `$expand`。 |
|transitiveMemberOf |[directoryObject](directoryobject.md) collection| 此设备所属的组和管理单元。 此操作是可传递的。 支持 `$expand`。  |
|usageRights|[usageRight](usageright.md) 集合|表示已授予设备的使用权限。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "approximateLastSignInDateTime": "String (timestamp)",
  "complianceExpirationDateTime": "String (timestamp)",
  "deviceCategory": "string",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceOwnership": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "domainName": "string",
  "enrollmentProfileName": "string",
  "enrollmentType": "string",
  "extensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "isRooted": true,
  "mdmAppId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "profileType": "string",
  "registrationDateTime": "String (timestamp)",
  "systemLabels": ["string"],
  "hostNames" : ["string"],
  "trustType": "string",
  "Name": "string",
  "Status": "string",
  "Platform": "string",
  "Kind": "string",
  "Model": "string",
  "managementType": "string",
  "Manufacturer": "string"
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
