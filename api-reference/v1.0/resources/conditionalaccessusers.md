---
title: conditionalAccessUsers 资源类型
description: 表示策略作用域中包括和排除的用户、组和角色。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8f75eb86ab9627b2cb9d507de9321743524203b3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129770"
---
# <a name="conditionalaccessusers-resource-type"></a>conditionalAccessUsers 资源类型

命名空间：microsoft.graph

表示策略作用域中包括和排除的用户、组和角色。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeUsers | String collection | 策略范围内的用户 ID（除非明确排除）或 `None` 或 `All` `GuestsOrExternalUsers` 。 |
| excludeUsers | String collection | 策略作用域中排除的用户 ID 和/或 `GuestsOrExternalUsers` 。 |
| includeGroups | String collection | 策略作用域中的组 ID（除非明确排除）或 `All` 。 |
| excludeGroups | String collection | 从策略作用域中排除的组 ID。 |
| includeRoles | String collection | 策略作用域中的角色 ID（除非明确排除）或 `All` 。 |
| excludeRoles | String collection | 从策略作用域排除的角色 ID。 |

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

