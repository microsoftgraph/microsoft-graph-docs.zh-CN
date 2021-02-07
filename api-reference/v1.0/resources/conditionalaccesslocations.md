---
title: conditionalAccessLocations 资源类型
description: 表示包含在策略作用域中和从策略范围中排除的位置。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 670f07e22b2027c74a79eaca505c624c04c19621
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132112"
---
# <a name="conditionalaccesslocations-resource-type"></a>conditionalAccessLocations 资源类型

命名空间：microsoft.graph

表示包含在策略作用域中和从策略范围中排除的位置。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeLocations | String collection | 除非明确排除，否则策略范围内的位置 `All` ID 或 `AllTrusted` 。 |
| excludeLocations | String collection | 从策略作用域中排除的位置 ID。 |

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

