---
title: conditionalAccessUsers 资源类型
description: 代表策略作用域中包含和排除的用户、组和角色。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7e54c5b018331952776b36a0ab3c07be88c2be7c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638475"
---
# <a name="conditionalaccessusers-resource-type"></a>conditionalAccessUsers 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表策略作用域中包含和排除的用户、组和角色。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeUsers | String collection | 策略作用域中的用户 Id，除非明确排除`None`或`All`或`GuestsOrExternalUsers`或。 |
| excludeUsers | String collection | 从策略作用域和/或`GuestsOrExternalUsers`中排除的用户 id。 |
| includeGroups | String collection | 除非明确排除或`All`，否则策略作用域中的组 id。 |
| excludeGroups | String collection | 从策略作用域中排除的组 Id。 |
| includeRoles | String collection | 策略作用域中的角色 Id，除非明确排除`All`或。 |
| excludeRoles | String collection | 从策略范围中排除的角色 Id。 |

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