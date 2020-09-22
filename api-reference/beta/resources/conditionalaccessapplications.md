---
title: conditionalAccessApplications 资源类型
description: 表示策略作用域中包含和排除的应用程序和用户操作。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d5a25b287d4f82aaaf9a7773893f96a02a7cf124
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085190"
---
# <a name="conditionalaccessapplications-resource-type"></a>conditionalAccessApplications 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示策略中包含和排除的应用程序和用户操作。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| includeApplications | 字符串集合 | 该策略应用于的应用程序 Id 列表，除非在 excludeApplications) 中显式排除 (。 也可以将设置为 `All` 。 |
| excludeApplications | 字符串集合 | 从策略中显式排除的应用程序 Id 的列表。 |
| includeUserActions | 字符串集合 | 要包括的用户操作 (例如 `urn:user:registersecurityinfo`)  |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

