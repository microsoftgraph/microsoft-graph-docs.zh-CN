---
title: targetResourcePolicy 资源类型
description: '指示已受影响的审核活动的策略。 派生 targetResource 资源。   '
ms.openlocfilehash: 20486c535d0df4b3745f5cfc3414b320a9374075
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046754"
---
# <a name="targetresourcepolicy-resource-type"></a>targetResourcePolicy 资源类型
指示已受影响的审核活动的策略。 派生[targetResource](targetresource.md)资源。   



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|policyType|字符串|指示已更改或已更改的设定的策略名称|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourcePolicy"
}-->

```json
{
  "policyType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourcePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->