---
author: JeremyKelley
description: publicationFacet 资源提供有关 driveItemVersion 或 driveItem 资源发布状态的详细信息。
ms.date: 09/10/2017
title: PublicationFacet
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 066c0c03a436acff42f4186183b483d76afceffa
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176743"
---
# <a name="publicationfacet-resource-type"></a>PublicationFacet 资源类型

命名空间：microsoft.graph

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

|   属性    |  类型  | Description |
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


