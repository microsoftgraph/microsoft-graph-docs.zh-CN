---
title: sectionGroup 资源类型
description: OneNote 笔记本中的分区组。分区组可以包含分区和分区组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 65e420d014add658a538deb42c01518cd94d611c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523706"
---
# <a name="sectiongroup-resource-type"></a>sectionGroup 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneNote 笔记本中的分区组。分区组可以包含分区和分区组。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|创建项的用户、设备和应用程序标识。只读。|
|createdDateTime|DateTimeOffset|分区组的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|id|字串符号|分区组的唯一标识符。只读。|
|lastModifiedBy|[identitySet](identityset.md)|识别创建项目的用户、设备和应用程序。只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改分区组的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|displayName|String|分区组的名称。|
|sectionGroupsUrl|String|`sectionGroups` 导航属性的 URL，其将返回分区组中的所有分区组。只读。|
|sectionsUrl|String|`sections` 导航属性的 URL，其将返回分区组中的所有分区。只读。|
|self|字符串|可以在其中获取关于分区阻的详细信息的终结点。只读。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|包含分区组的笔记本。只读。|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|包含分区组的分区组。只读。|
|sectionGroups|[SectionGroup](sectiongroup.md) collection|分区中的分区组。只读。可为 NULL。|
|节|[Section](section.md) collection|分区组中的分区。只读。可为 Null。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get section group](../api/sectiongroup-get.md) | [SectionGroup](sectiongroup.md) |读取分区组的属性和关系。|
|[Create section group](../api/sectiongroup-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| 通过发布到指定分区组中的 sectionGroups 集合创建分区组。|
|[List section groups](../api/sectiongroup-list-sectiongroups.md) |[SectionGroup](sectiongroup.md) collection| 获取指定分区组中的分区组集合。|
|[Create section](../api/sectiongroup-post-sections.md) |[Section](section.md)| 通过发布到指定分区组中的分区集合创建分区。|
|[List sections](../api/sectiongroup-list-sections.md) |[Section](section.md) collection| 获取指定分区组中的分区集合。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sectiongroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
