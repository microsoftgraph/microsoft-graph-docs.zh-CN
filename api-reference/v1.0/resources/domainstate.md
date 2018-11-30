---
title: domainState 资源类型
description: 表示域上经过计划的异步操作的状态。
ms.openlocfilehash: 73a83eddb46b9305a6d74e283bae1c009361195d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010142"
---
# <a name="domainstate-resource-type"></a>domainState 资源类型

表示域上经过计划的异步操作的状态。

## <a name="properties"></a>属性

| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | 上个活动发生时的时间戳。计划操作、异步任务启动及操作完成后将更新此值。 |
| 操作 | String | 异步操作类型。其值可以为 *ForceDelete* 或 *Verification*。 |
| status | String | 操作的当前状态。 <br> *Scheduled* - 已计划操作但尚未启动。 <br> *InProgress* - 任务已启动并且正在进行中。 <br> *Failed* - 操作已失败。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->