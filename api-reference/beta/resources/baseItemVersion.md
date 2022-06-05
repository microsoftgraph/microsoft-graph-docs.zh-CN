---
author: JeremyKelley
description: baseItemVersion 资源表示项或实体的以前版本。
ms.date: 09/17/2017
title: BaseItemVersion
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: fb1383c2e906b17c039d0489c5212f7084f8c2f2
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899419"
---
# <a name="baseitemversion-resource-type"></a>BaseItemVersion 资源类型

命名空间：microsoft.graph

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

| 属性                 | 类型                                                 | 说明                                                             |
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
  "suppressions": []
}
-->
