---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 22bf6b1101be9d60ff350e0b04f7627e2b8fb529
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524028"
---
# <a name="sharepointids-resource-type"></a>SharePointIds 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**SharePointIds** 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。

**注意：** OneDrive 个人版返回的项将不包括 **SharePointIds** 方面。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "tenantId": "string",
    "webId": "string"
}
```

## <a name="properties"></a>属性

| 属性         | 类型         | 说明
|:-----------------|:-------------|:-------------------------------------------
| listId           | string       | SharePoint 中的项列表的唯一标识符 (guid)。
| listItemId       | string       | 包含列表中的项的整数标识符。
| listItemUniqueId | string       | OneDrive for Business 或 SharePoint 网站中的项的唯一标识符 (guid)。
| siteId           | string       | 项的网站集 (SPSite) 的唯一标识符 (guid)。
| siteUrl          | string (url) | 包含项的网站的 SharePoint URL。
| tenantId         | string       | 租户的唯一标识符 (guid)。
| webId            | string       | 项的网站集 (SPWeb) 的唯一标识符 (guid)。

## <a name="remarks"></a>注解

有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepointids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
