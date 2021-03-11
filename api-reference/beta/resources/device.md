---
title: 设备资源类型
description: 表示在目录中注册的设备。
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: fa201a61b1b2dd126cd75a9e90be1f6ec4b34d5e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721641"
---
# <a name="device-resource-type"></a>设备资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在目录中注册的设备。 可以在云中使用设备注册服务或 Intune 创建设备。 条件访问策略使用它们进行多重身份验证。 这些设备范围很广，从台式机、笔记本电脑到手机和平板电脑均包括在内。 继承自 [directoryObject](directoryobject.md)。

使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取设备](../api/device-get.md) | [设备](device.md) |读取设备对象的属性和关系。|
|[列出设备](../api/device-list.md) | [设备](device.md) 集合| 检索目录中的注册设备列表。 |
|[更新设备](../api/device-update.md) | [设备](device.md)  |更新设备对象的属性。 |
|[删除设备](../api/device-delete.md) | 无 |删除设备对象。 |
|[List memberOf](../api/device-list-memberof.md) |[directoryObject](directoryobject.md) 集合| 列出设备是其直接成员中的组。 |
|[列出 transitive memberOf](../api/device-list-transitivememberof.md) |[directoryObject](directoryobject.md) 集合| 列出设备是其中一个成员的组。 此操作是可传递的。 |
|[列出 registeredOwners](../api/device-list-registeredowners.md) |[directoryObject](directoryobject.md) 集合| 通过 registeredOwners 导航属性，获取身份为设备注册所有者的用户。|
|[列出 registeredUsers](../api/device-list-registeredusers.md) |[directoryObject](directoryobject.md) 集合| 从 registeredUsers 导航属性获取设备的注册用户。|
|[列表 usageRights](../api/device-list-usagerights.md) | [usageRight](usageright.md) 集合 | 获取授予设备的使用权限的集合。|
|[checkMemberObjects](../api/device-checkmemberobjects.md) | String 集合 | 检查组、目录角色或管理单元对象列表中的成员身份。 |
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accountEnabled|布尔| 启用帐户时为 **true**，否则为 **false**。 默认值为 true。|
|alternativeSecurityIds|alternativeSecurityId 集合| 仅供内部使用。 不可为 null。 |
|approximateLastSignInDateTime|DateTimeOffset| 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
|complianceExpirationDateTime|DateTimeOffset| 设备不再被视为合规的时间戳。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
|deviceCategory|String|Intune 设置的用户定义属性，用于自动将设备添加到组并简化设备管理。|
|deviceId|Guid| 由 Azure 设备注册服务在设备注册时设置的唯一标识符。 |
|deviceMetadata|String| 仅供内部使用。 设置为 null。 |
|deviceOwnership|String|设备的所有权。 此属性由 Intune 设置。 可能的值包括：unknown、company、personal。|
|deviceVersion|Int32| 仅供内部使用。 |
|displayName|String| 设备显示名称。必需。 |
|domainName|String|已加入混合 Azure AD 设备的本地域名。 此属性由 Intune 设置。|
|enrollmentProfileName|String|应用于设备的注册配置文件。 例如，Apple 设备注册配置文件、设备注册 - 公司设备标识符或 Windows Autopilot 配置文件名称。 此属性由 Intune 设置。|
|enrollmentType|String|设备的注册类型。 此属性由 Intune 设置。 可能的值包括：unknown、userEnrollment、deviceEnrollmentManager、appleBulkWithUser、appleBulkWithoutUser、windowsAzureADJoin、windowsBulkUserless、windowsAutoEnrollment、windowsBulkAzureDomainJoin、windowsCoManagement。|
|id|String|设备唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL。只读。|
|isCompliant|Boolean|如果设备符合移动设备管理 (MDM) 策略，则为 **true**；否则；为 **false**。 只读。 这只能由 Intune 针对任何设备操作系统类型进行更新，或由适用于 Windows OS 设备的已批准 [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) 应用更新。|
|isManaged|Boolean|如果设备由移动设备管理 (MDM) 应用进行托管，则为 **true**；否则，为 **false**。 这只能由 Intune 针对任何设备操作系统类型进行更新，或由适用于 Windows OS 设备的已批准 [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) 应用更新。 |
|isRooted|布尔|如果设备为根，则 **其为 true;****假** 如果设备已越狱。 这只能由 Intune 更新。|
|managementType|String|设备的管理通道。  此属性由 Intune 设置。 可能的值是：eas、mdm、easMdm、intuneClient、easIntuneClient、configurationManagerClient、configurationManagerClientMdm、configurationManagerClientMdmEas、unknown、jamf、googleCloudDevicePolicyController。|
|manufacturer|String| 设备的制造商。 只读。 |
|mdmAppId|String|用于将设备注册到 MDM 的应用程序标识符。 <br><br>只读。 支持 $filter。|
|model|String| 设备型号。 只读。 |
|onPremisesLastSyncDateTime|DateTimeOffset|上次将对象与本地目录同步的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC `2014-01-01T00:00:00Z` 为只读。 |
|onPremisesSyncEnabled|Boolean|如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。 只读。|
|operatingSystem|String| 设备上操作系统的类型。必需。 |
|operatingSystemVersion|String| 设备的操作系统版本。 必需。 |
|physicalIds|String collection| 仅供内部使用。 不可为 null。 |
|profileType|String|设备的配置文件类型。 可能的值：<br />**RegisteredDevice (** 默认) <br />**SecureVM**<br />**Printer**<br />**共享**<br />**IoT**|
|registrationDateTime|DateTimeOffset|设备注册的日期和时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|systemLabels|字符串集合| 系统应用于设备的标签列表。 |
|hostNames|字符串集合| 设备的 hostNames 列表。|
|trustType|String| 加入设备的信任类型。 只读。 可取值为： <br />**Workplace** - 表示 *自带个人设备*<br />**AzureAd** - 仅云加入设备<br />**ServerAd** - 加入 Azure AD 的本地域加入设备。 如需了解更多详情，请参阅 [Azure Active Directory 中的设备管理简介](/azure/active-directory/device-management-introduction) |
|名称| String | 设备的友好名称。 仅在用户使用 Microsoft 帐户登录作为 Project Rome 的一部分时返回。 |
|状态 | String| 设备处于联机或脱机状态。 仅在用户使用 Microsoft 帐户登录作为 Project Rome 的一部分时返回。 |
|平台 |String|设备平台。 仅在用户使用 Microsoft 帐户登录作为 Project Rome 的一部分时返回。 仅在用户使用 Microsoft 帐户登录作为 Project Rome 的一部分时返回。|
|Kind| 字符串| 设备的外形要求。 仅在用户使用 Microsoft 帐户登录作为 Project Rome 的一部分时返回。 |
|模型| String| 设备型号。 仅在用户使用 Microsoft 帐户登录作为 Project Rome 的一部分时返回。 |
|制造商| String| 设备制造商。 仅在用户使用 Microsoft 帐户登录作为 Project Rome 的一部分时返回。 |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|extensions|[扩展](extension.md)集合|为设备定义的开放扩展集合。只读。可为 NULL。|
|registeredOwners|[directoryObject](directoryobject.md) 集合| 云加入设备或已注册个人设备的用户。 已注册的所有者是在注册时设置。 目前，只能有一个所有者。 只读。 可为 NULL。|
|registeredUsers|[directoryObject](directoryobject.md) 集合| 设备的已注册用户集合。 对于云加入设备和已注册的个人设备，已注册用户在设备注册时设置为与已注册所有者相同的值。 只读。 可为 NULL。|
|extensions|[扩展](extension.md)集合|为设备定义的开放扩展的集合。 可为 NULL。|
| 命令 | [命令](command.md) 集合 | 发送到此设备的命令集|
|usageRight|[usageRight](usageright.md) 集合|表示已授予设备的使用权限。 |

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
