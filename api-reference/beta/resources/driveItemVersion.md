---
author: JeremyKelley
description: DriveItemVersion 资源表示特定版本的 DriveItem。
ms.date: 09/17/2017
title: DriveItemVersion
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: d6f2245fe02657d883d1e6646ac6ff6fce0187ea
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723160"
---
# <a name="driveitemversion-resource-type"></a>DriveItemVersion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**DriveItemVersion** 资源表示特定版本的 [DriveItem](driveitem.md)。

## <a name="tasks-on-driveitemversion-resources"></a>DriveItemVersion 资源上的任务

下列任务可用于 driveItemVersion 资源。

| 常见任务                        | HTTP 方法                                                        |
| :--------------------------------- | :----------------------------------------------------------------- |
| [列出版本][version-list]      | `GET /drive/items/{item-id}/versions`                              |
| [获取版本][version-get]         | `GET /drive/items/{item-id}/versions/{version-id}`                 |
| [获取内容][content-get]        | `GET /drive/items/{item-id}/versions/{version-id}/content`         |
| [还原版本][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

在上表中，各示例使用的是 `/drive`，但有很多有效的请求。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource","keyProperty":"id", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": {"@odata.type": "Edm.Stream"},
  "id": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
  "size": 12356
}
```

## <a name="properties"></a>属性

| 属性                 | 类型                                                 | 说明                                                             |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | 版本 ID。 只读。                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | 上次修改版本的用户的标识。 只读。        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | 上次修改版本的日期和时间。 只读。                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | 指示此特定版本的发布状态。 只读。 |
| **size**                 | Int64                                                | 指示此版本项的内容流大小。  |

## <a name="relationships"></a>关系

下表定义了 **driveItemVersion** 资源与其他资源的关系。

| 关系 | 类型   | 说明                        |
| :----------- | :----- | :--------------------------------- |
| **content**  | Stream | 版本的内容流。 |

<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->
