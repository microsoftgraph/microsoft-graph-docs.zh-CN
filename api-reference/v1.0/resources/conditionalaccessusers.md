---
title: conditionalAccessUsers 资源类型
description: 代表策略作用域中包含和排除的用户、组和角色。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 460b14d88fcf153935948784c08a6d0a03d33553
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384495"
---
# <a name="conditionalaccessusers-resource-type"></a>conditionalAccessUsers 资源类型

命名空间：microsoft.graph

代表策略作用域中包含和排除的用户、组和角色。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeUsers | String collection | 策略作用域中的用户 Id，除非明确排除或 `None` 或或 `All` `GuestsOrExternalUsers` 。 |
| excludeUsers | String collection | 从策略作用域和/或中排除的用户 Id `GuestsOrExternalUsers` 。 |
| includeGroups | String collection | 除非明确排除或，否则策略作用域中的组 Id `All` 。 |
| excludeGroups | String collection | 从策略作用域中排除的组 Id。 |
| includeRoles | String collection | 策略作用域中的角色 Id，除非明确排除或 `All` 。 |
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
