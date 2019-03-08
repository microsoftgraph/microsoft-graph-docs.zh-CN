---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 66e12c3240d1cade57d377e43403b33102fe166e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482061"
---
# <a name="publicationfacet-resource-type"></a>PublicationFacet 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**publicationFacet** 资源提供有关 [driveItemVersion](driveitemversion.md) 或 [driveItem](driveitem.md) 资源发布状态的详细信息。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a>属性

|   属性    |  类型  | 说明 |
| :------------ | :----- | :---------- |
| **level**     | String | 此文档的发布状态。 `published` 或 `checkout`。 只读。  |
| **versionId** | String | 对当前调用方可见的版本的唯一标识符。 只读。  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicationfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
