---
title: governanceRuleSetting 资源类型
description: 表示角色设置所构成的规则。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 12436250814a45bae0c7bf3c910e01f2f0a0c303
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397476"
---
# <a name="governancerulesetting-resource-type"></a>governanceRuleSetting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

表示角色设置所构成的规则。


## <a name="properties"></a>属性
|属性      | 类型         |说明|
|:-------------|:-------------|:----------|
|ruleIdentifier|String        |规则的 ID。 例如， ``ExpirationRule`` 和 ``MfaRule``.|
|setting       |String        |规则的设置。 该值是一个 JSON 字符串，其中包含Parameter_Name：Parameter_Value格式的对列表。 例如，`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


