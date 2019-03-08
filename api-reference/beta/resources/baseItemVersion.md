---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 56a2c230c53c4b5bd50e8c123dd69eedec67a141
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480668"
---
# <a name="baseitemversion-resource-type"></a>BaseItemVersion 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**baseItemVersion** 资源表示项或实体的以前版本。


## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.baseItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>属性

|      属性名称       |                         类型                         |                               说明                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | 版本 ID。 只读。                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | 上次修改版本的用户的标识。 只读。        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | 上次修改版本的日期和时间。 只读。                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | 指示此特定版本的发布状态。 只读。 |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
