---
title: conditionalAccessLocations 资源类型
description: 表示包含在策略作用域中和从策略范围中排除的位置。
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e5e7de8a751c118a4d1a260a348a04ec1da2fb5
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161212"
---
# <a name="conditionalaccesslocations-resource-type"></a>conditionalAccessLocations 资源类型

命名空间：microsoft.graph

表示包含在策略作用域中和从策略范围中排除的位置。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeLocations | 字符串集合 | 除非明确排除 、或 ，否则策略范围内的位置 `All` `AllTrusted` ID。 |
| excludeLocations | 字符串集合 | 从策略作用域中排除的位置 ID。 |

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

