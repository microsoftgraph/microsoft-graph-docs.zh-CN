---
title: domainState 资源类型
description: 表示在域上计划的异步操作的状态。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 66d5d5b57cb5ef30054a6187e34caf8713b6e63b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505803"
---
# <a name="domainstate-resource-type"></a>domainState 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在域上计划的异步操作的状态。

## <a name="properties"></a>属性

| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | 上一次活动发生时的时间戳。 在计划工序、异步任务启动和操作完成时，会更新该值。 |
| 操作 | String | 异步操作的类型。 这些值可以是*ForceDelete*或*验证* |
| status | String | 操作的当前状态。 <br> *计划*-操作已计划，但尚未启动。 <br> *InProgress* -任务已启动并且正在进行中。 <br> *Failed* -操作失败。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
