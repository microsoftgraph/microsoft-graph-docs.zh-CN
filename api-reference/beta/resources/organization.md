---
title: 组织资源类型
description: '表示 Azure Active Directory 租户。 '
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f3a07629006f5f2cada6601dab09b952fdef7980
ms.sourcegitcommit: 6cea9bc17d3859e475a74c4a6f661f848e837e89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2021
ms.locfileid: "60240759"
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
|**组织许可证**| | |
|[activateService](../api/organization-activateservice.md) | 无 |  为组织激活服务。 |
|**组织品牌**| | |
|[Get organizationalBranding](../api/organizationalbranding-get.md) | [organizationalBranding](organizationalbranding.md) | 获取默认组织的品牌对象。 |
|[Update organizationalBranding](../api/organizationalbranding-update.md) | [organizationalBranding](organizationalbranding.md) | 更新默认组织的品牌对象。 |
|[创建 organizationalBrandingLocalization](../api/organizationalbranding-post-localizations.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | 创建新的本地化（特定语言的）品牌打造和默认品牌对象（如果不存在）。 |
|[List organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) 集合 | 检索租户中的所有本地化品牌对象。 |
|[Get organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | 读取本地化品牌对象的属性。 |
|[更新 organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | 更新本地化品牌对象。 |
|[删除 organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | 删除本地化品牌对象。 |
<!--|[Delete organizationalBranding](../api/organizationalbranding-update.md) | [organizationalBranding](organizationalbranding.md) | 删除默认组织的品牌对象。 |

**NOTE： To restore the Delete organizationalBranding operation back into the table after Update organizationalBranding if all inconsistencies are resolved.-->

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:-------- |:---- |:----------- |
| assignedPlans | [assignedPlan](assignedplan.md) 集合 | 与租户相关的服务计划的集合。不可为空。 |
| businessPhones | String collection | 组织的电话号码。虽然这是字符串集合，但是只能为该属性设置一个号码。 |
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
| onPremisesSyncEnabled | Boolean | `true` 如果此对象从本地目录同步; `false` 如果此对象最初从本地目录同步，但不再同步;可为空。 `null` 如果此对象从未从本地目录（默认）进行同步。 |
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
|extensions|[扩展](extension.md)集合|为组织资源定义的开放扩展集合。 可为 Null。| 
|organizationalbranding|[organizationalBranding](organizationalbranding.md) 集合| 用于管理组织的默认品牌的资源。 可为 Null。|
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
  "businessPhones": ["String"],
  "city": "String",
  "country": "String",
  "countryLetterCode": "String",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "directorySizeQuota": {"@odata.type": "microsoft.graph.directorySizeQuota"},
  "displayName": "String",
  "id": "String (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "Boolean",
  "marketingNotificationEmails": ["String"],
  "objectType": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "String",
  "preferredLanguage": "String",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["String"],
  "securityComplianceNotificationPhones": ["String"],
  "state": "String",
  "street": "String",
  "technicalNotificationMails": ["String"],
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
