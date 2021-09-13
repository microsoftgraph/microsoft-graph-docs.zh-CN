---
title: conditionalAccessLocations 资源类型
description: 表示包含在策略作用域中和从策略范围中排除的位置。
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 68804b5728fd058d2502ac041a24c3a218692b93
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109245"
---
# <a name="conditionalaccesslocations-resource-type"></a>conditionalAccessLocations 资源类型

命名空间：microsoft.graph

表示包含在策略作用域中和从策略范围中排除的位置。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeLocations | 字符串集合 | 除非明确排除 、或 ，否则策略范围内的位置 `All` `AllTrusted` ID。 |
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

