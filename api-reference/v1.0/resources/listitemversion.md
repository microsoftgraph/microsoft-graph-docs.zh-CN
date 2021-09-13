---
title: ListItemVersion 资源类型
description: '**listItemVersion** 资源表示先前版本的 ListItem 资源。'
ms.localizationpriority: medium
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: 3b8881ed9e2fbf13176562f25397e5596a25257a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062465"
---
# <a name="listitemversion-resource-type"></a>ListItemVersion 资源类型

命名空间：microsoft.graph

**listItemVersion** 资源表示先前版本的 [ListItem](listitem.md) 资源。

## <a name="tasks-on-listitemversion-resources"></a>ListItemVersion 资源上的任务

下列任务可用于 listItemVersion 资源。

|            常见任务             |         HTTP 方法         |
| :--------------------------------- | :-------------------------- |
| [列出版本][version-list]      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| [获取版本][version-get]         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| [还原版本][version-restore] | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a>JSON 表示形式

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka&quot;: &quot;oneDrive.baseItemVersion"
}-->

```json
{
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


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->

