---
title: conditionalAccessFilter 资源类型
description: 表示策略作用域中的筛选器。
ms.localizationpriority: medium
author: sandeo
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 62c0c21a01a67bbaf08fae16fcb4f0d7451efe9a
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995413"
---
# <a name="conditionalaccessfilter-resource-type"></a>conditionalAccessFilter 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示策略作用域中的筛选器。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| mode | filterMode | 用于筛选器的模式。 可能的值为 `include` 或 `exclude`。 |
| rule | 字符串 | 规则语法类似于用于组中组成员身份规则的Azure Active Directory。 有关详细信息，请参阅 [包含多个表达式的规则](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions) |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "mode",
    "rule"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessFilter",
  "baseType": null
}-->

```json
{
  "mode": "String",
  "rule": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessFilter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


