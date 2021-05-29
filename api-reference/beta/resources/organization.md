---
title: 组织资源类型
description: '表示 Azure Active Directory 租户。 '
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 984fff26922d2300b94af69f3263e2beaeab82f8
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703592"
---
# <a name="organization-resource-type"></a>组织资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户或应用程序所登录的 Azure Active Directory 租户。 只支持在此资源上执行读取和更新操作；不支持创建和删除操作。 继承自 [directoryObject](directoryobject.md)。

使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取组织](../api/organization-get.md) | [organization](organization.md) 集合|读取 organization 对象的属性和关系。|
|[更新 organization](../api/organization-update.md) | [组织](organization.md)  |更新 organization 对象。 可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。 |
| [获取组织设置](../api/organizationsettings-get.md) | [organizationSettings](organizationsettings.md) | 读取组织设置对象。 |
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](../api/schemaextension-post-schemaextensions.md) | [schemaExtension](schemaextension.md) | 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|
|[创建 organizationalBrandingProperties](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | 通过发布到品牌集合创建新的 organizationalBrandingProperties。 |
|[进行品牌打造](../api/organizationalbrandingproperties-get.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) 集合 | 获取 organizationalBrandingProperties 对象集合。 |

## <a name="properties"></a>属性 
| 属性 | 类型   | 说明 |
|:-------- |:---- |:----------- |
| assignedPlans | [assignedPlan](assignedplan.md) 集合 | 与租户相关的服务计划的集合。不可为空。 |
| businessPhones | 字符串集合 | 组织的电话号码。 虽然这是字符串集合，但是只能为该属性设置一个号码。 |
| 城市 | String | 组织地址所在的城市名称。 |
| country | String | 组织地址所在的国家/地区名称。 |
| countryLetterCode | String | 组织所在的国家/地区缩写。 |
| createdDateTime | DateTimeOffset | 组织的创建时间戳。 值无法修改，并在组织创建时自动填充。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
| deletedDateTime | DateTimeOffset | 表示采用 ISO 8601 格式创建 Azure AD 的日期和时间，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
| directorySizeQuota | [directorySizeQuota](directorySizeQuota.md) | 组织的目录大小配额信息。 |
| displayName | String | 租户的显示名称。 |
| id | 字符串 | 租户 ID，表示组织（或租户）的唯一标识符。 继承自 [directoryObject](directoryobject.md)。 键。 不可为 null。 只读。 |
| isMultipleDataLocationsForServicesEnabled | 布尔值 | `true` 如果组织已启用多地理位置; `false` 如果组织未启用多地理位置; `null` (默认) 。 只读。 有关详细信息，请参阅 [OneDrive Online 多地理位置](/sharepoint/dev/solution-guidance/multigeo-introduction)。 |
| marketingNotificationEmails | String collection | 不可为空。 |
| objectType | String | 一个标识对象类型的字符串。 对于租户，该值始终为 `Company` 。|
| onPremisesLastSyncDateTime | DateTimeOffset | 租户上次与本地目录同步的时间和日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
| onPremisesSyncEnabled | 布尔 | `true` 如果此对象从本地目录同步; `false` 如果此对象最初从本地目录同步，但不再同步;可为空。 `null` 如果此对象从未从本地目录（默认）进行同步。 |
| postalCode | String | 组织地址的邮政编码。 |
| preferredLanguage | String | 组织的首选语言。 应遵循 ISO 639-1 代码;例如， `en`。 |
| privacyProfile | [privacyProfile](privacyprofile.md) | 组织的隐私配置文件。 |
| provisionedPlans | [provisionedPlan](provisionedplan.md) 集合 | 不可为 null。 |
| securityComplianceNotificationMails | String collection ||
| securityComplianceNotificationPhones | String collection ||
| state | String | 组织地址所在的省/自治区/直辖市名称。 |
| street | String | 组织地址所在的街道名称。 |
| technicalNotificationMails |String collection | 不可为空。 |
| verifiedDomains | [verifiedDomain](verifieddomain.md) 集合|与该租户相关联的域集合。不可为 null。 |

## <a name="relationships"></a>关系

| 关系  | 类型  |说明|
|:---------------|:--------|:----------|
|certificateBasedAuthConfiguration|[certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) 集合| 用于管理基于证书的身份验证配置的导航属性。 只能在集合中创建 certificateBasedAuthConfiguration 的单个实例。  |
|extensions|[扩展](extension.md)集合|为组织资源定义的开放扩展集合。 可为 NULL。| 
|organizationalbranding|[organizationalBrandingProperties](organizationalbrandingproperties.md) 集合| 为组织打造品牌。 可为 Null。|
|settings|[organizationSettings](organizationsettings.md) | 检索 organizationSettings 对象的属性和关系。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "directorySizeQuota": {"@odata.type": "microsoft.graph.directorySizeQuota"},
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
  "marketingNotificationEmails": ["string"],
  "objectType": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}],
  "companyLastDirSyncTime": "2019-02-07T20:33:52.942Z",
  "dirSyncEnabled": true
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
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
