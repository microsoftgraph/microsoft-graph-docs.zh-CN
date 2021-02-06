---
title: conditionalAccessUsers 资源类型
description: 表示策略作用域中包括和排除的用户、组和角色。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6214c3daacf580aaffa01a93be2b2c785c03f4fd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128580"
---
# <a name="conditionalaccessusers-resource-type"></a>conditionalAccessUsers 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示策略作用域中包括和排除的用户、组和角色。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeUsers | 字符串集合 | 策略范围内的用户 ID（除非明确排除）或 `None` 或 `All` `GuestsOrExternalUsers` 。 |
| excludeUsers | 字符串集合 | 策略作用域中排除的用户 ID 和/或 `GuestsOrExternalUsers` 。 |
| includeGroups | 字符串集合 | 策略作用域中的组 ID（除非明确排除）或 `All` 。 |
| excludeGroups | 字符串集合 | 从策略作用域中排除的组 ID。 |
| includeRoles | 字符串集合 | 策略作用域中的角色 ID（除非明确排除）或 `All` 。 |
| excludeRoles | 字符串集合 | 从策略作用域排除的角色 ID。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeUsers",
    "excludeUsers",
    "includeGroups",
    "excludeGroups",
    "includeRoles",
    "excludeRoles"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessUsers",
  "baseType": null
}-->

```json
{
  "excludeGroups": ["String"],
  "excludeRoles": ["String"],
  "excludeUsers": ["String"],
  "includeGroups": ["String"],
  "includeRoles": ["String"],
  "includeUsers": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessUsers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

