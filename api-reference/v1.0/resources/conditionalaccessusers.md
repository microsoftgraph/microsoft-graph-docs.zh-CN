---
title: conditionalAccessUsers 资源类型
description: 表示包含在策略作用域中和从策略作用域中排除的用户、组和角色。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9f9930d1d1ac1b5d355699b893bfbf59f047162d1d0c0f39d0303a98b889ab7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229302"
---
# <a name="conditionalaccessusers-resource-type"></a>conditionalAccessUsers 资源类型

命名空间：microsoft.graph

表示包含在策略作用域中和从策略作用域中排除的用户、组和角色。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeUsers | String collection | 除非明确排除或 或 ，否则策略范围中的用户 `None` `All` `GuestsOrExternalUsers` ID。 |
| excludeUsers | String collection | 策略作用域中排除的用户 ID 和/或 `GuestsOrExternalUsers` 。 |
| includeGroups | String collection | 除非明确排除 或 ，否则策略作用域中的组 `All` ID。 |
| excludeGroups | String collection | 策略作用域中排除的组 ID。 |
| includeRoles | String collection | 除非明确排除 或 ，否则在策略作用域中的角色 `All` ID。 |
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

