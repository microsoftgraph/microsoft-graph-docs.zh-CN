---
title: conditionalAccessApplications 资源类型
description: 表示策略作用域中包含和排除的应用程序和用户操作。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3d864acfdd794bc5bcb914c460b29800c4a86291
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962502"
---
# <a name="conditionalaccessapplications-resource-type"></a>conditionalAccessApplications 资源类型

命名空间：microsoft.graph

表示包含在策略中和从策略中排除的应用程序和用户操作。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeApplications | String collection | 除非在 excludeApplications (中明确排除策略所适用的应用程序) 。 也可以设置为 `All` 。 |
| excludeApplications | String collection | 从策略中显式排除的应用程序 ID 列表。 |
| includeUserActions | String collection | 要包含的用户操作。 支持的值 `urn:user:registersecurityinfo` 包括 和 `urn:user:registerdevice` |

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

