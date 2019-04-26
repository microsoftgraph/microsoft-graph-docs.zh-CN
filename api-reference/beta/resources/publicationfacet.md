---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: a95ec524b8e33ce65d9ecb7030a90a49305cdf6c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344058"
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
  "suppressions": []
}
-->
