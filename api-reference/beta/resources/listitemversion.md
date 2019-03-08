---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d9b06b54d12abddd3a1586a11b99f7c600ac4508
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482299"
---
# <a name="listitemversion-resource-type"></a>ListItemVersion 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**listItemVersion** 资源表示先前版本的 [ListItem](listitem.md) 资源。

## <a name="tasks-on-listitemversion-resources"></a>ListItemVersion 资源上的任务

下列任务可用于 listItemVersion 资源。

|            常见任务             |         HTTP 方法         |
| :--------------------------------- | :-------------------------- |
| [列出版本][version-list]      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| [获取版本][version-get]         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| [还原版本][version-restore] | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>属性

|      属性名称       |                         类型                         |                               说明                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | 版本 ID。 只读。                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | 上次修改版本的用户的标识。 只读。        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | 上次修改版本的日期和时间。 只读。                 |
| **published**            | [PublicationFacet](../resources/publicationfacet.md) | 指示此特定版本的发布状态。 只读。 |


## <a name="relationships"></a>关系

下表定义了 **driveItemVersion** 资源与其他资源的关系。

| 关系名称 |                      类型                      |                               说明                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| **fields**        | [FieldValueSet](../resources/fieldvalueset.md) | 此版本列表项的字段和值集合。 |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/listitemversion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
