---
title: 联系人资源类型
description: 联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8833fca292efffc631f190b0f9e201d5f0d02929
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014031"
---
# <a name="contact-resource-type"></a>联系人资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。

该资源支持：

- 将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/contact-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法
| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取联系人](../api/contact-get.md) | [联系人](contact.md) |读取 contact 对象的属性和关系。|
|[创建](../api/user-post-contacts.md) | [联系人](contact.md) |将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。|
|[更新](../api/contact-update.md) | [联系人](contact.md) |更新 contact 对象。 |
|[删除](../api/contact-delete.md) | 无 |删除 contact 对象。 |
|[delta](../api/contact-delta.md)|[联系人](contact.md)集合| 获取指定文件夹中已添加、删除或更新的联系人集。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[联系人](contact.md)  |在新建或现有的联系人中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的联系人](../api/singlevaluelegacyextendedproperty-get.md)  | [联系人](contact.md) | 通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的联系人。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [联系人](contact.md) | 在新建或现有的联系人中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的联系人](../api/multivaluelegacyextendedproperty-get.md)  | [联系人](contact.md) | 使用 `$expand` 获取包含一个多值扩展属性的联系人。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assistantName|String|联系人助理的姓名。|
|birthday|DateTimeOffset|联系人的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|categories|String collection|与联系人关联的类别。 每个类别对应于为用户定义的 [outlookCategory](outlookcategory.md) 的 **displayName** 属性。|
|changeKey|String|标识联系人的版本。每次联系人更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。|
|children|String collection|联系人子女的姓名。|
|companyName|String|联系人所在公司的名称。|
|createdDateTime|DateTimeOffset|创建联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|department|String|联系人所在的部门。|
|displayName|String|联系人的显示名称。 可以在[创建](../api/user-post-contacts.md)或[更新](../api/contact-update.md)操作中指定显示名称。 请注意，对其他属性的后续更新可能会导致自动生成的值覆盖你指定的 displayName 值。 若要保留预先存在的值，请始终在[更新](../api/contact-update.md)操作中将其作为 displayName。|
|emailAddresses|[typedEmailAddress](typedemailaddress.md) 集合|联系人的电子邮件地址。|
|fileAs|String|联系人备案的姓名。|
|flag|[followupFlag](followupflag.md)|指示联系人的状态、开始日期、截止日期或完成日期的标志值。 |
|gender |String |联系人的性别。 |
|generation|String|联系人所属的代。|
|givenName|String|联系人的名。|
|id|String| 联系人的唯一标识符。 [!INCLUDE [outlook-beta-id](../../includes/outlook-immutable-id.md)] 只读。 |
|imAddresses|String collection|联系人的即时消息 (IM) 地址。|
|initials|String|联系人的姓名缩写。|
|jobTitle|String|联系人的职务。|
|lastModifiedDateTime|DateTimeOffset|修改联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|manager|String|联系人经理的姓名。
|middleName|String|联系人的中间名。|
|nickName|String|联系人的昵称。|
|officeLocation|String|联系人的办公室位置。|
|parentFolderId|String|联系人的父文件夹 ID。|
|personalNotes|String|有关联系人的用户备注。|
|phones |[phone](phone.md) collection |电话联系人关联的电话号码，例如住宅电话、移动电话和业务电话。 |
|postalAddresses |[physicalAddress](physicaladdress.md) 集合 |与联系人关联的地址，例如，住宅地址和公司地址。 |
|profession|String|联系人的职业。|
|spouseName|String|联系人配偶/伴侣的姓名。|
|surname|String|联系人的姓氏。|
|title|String|联系人的职位。|
|websites |[website](website.md) collection|与联系人关联的网站。 |
|将anniversary |Date |联系人的周年日。 |
|yomiCompanyName|String|联系人的注音日文公司名称。|
|yomiGivenName|String|联系人的注音日文名字。|
|yomiSurname|String|联系人的注音日文姓氏。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|extensions|[扩展](extension.md)集合|为联系人定义的开放扩展集合。 可为 Null。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为联系人定义的多值扩展属性的集合。只读。可为 Null。|
|photo|[照片](profilephoto.md)| 可选的联系人照片。可以获取或设置联系人的照片。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为联系人定义的单值扩展属性的集合。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.typedEmailAddress"}],
  "fileAs": "string",
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "gender": "string",
  "generation": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "nickName": "string",
  "officeLocation": "string",
  "parentFolderId": "string",
  "personalNotes": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.physicalAddress"}],
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "weddingAnniversary": "date",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string"
}
```

## <a name="see-also"></a>另请参阅

- [使用增量查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)
- [获取文件夹中邮件的增量更改](/graph/delta-query-messages)
- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


