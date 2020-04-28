---
title: conditionalAccessLocations 资源类型
description: 表示策略作用域中包含和排除的位置。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a92d99d7a9e80084b8ec1ce385ce76d1f522b359
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916780"
---
# <a name="conditionalaccesslocations-resource-type"></a>conditionalAccessLocations 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示策略作用域中包含和排除的位置。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeLocations | String 集合 | 除非明确排除、 `All`或`AllTrusted`，否则策略范围中的位置 id。 |
| excludeLocations | String 集合 | 从策略范围中排除的位置 Id。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

## <a name="relationships"></a>关系

无。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeLocations",
    "excludeLocations"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessLocations",
  "baseType": null
}-->

```json
{
  "excludeLocations": ["String"],
  "includeLocations": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessLocations resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->