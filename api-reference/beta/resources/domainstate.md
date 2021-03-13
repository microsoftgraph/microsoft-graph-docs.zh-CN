---
title: domainState 资源类型
description: 表示在域中安排的异步操作的状态。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 15189beb4441d606becc470f4fb3fbe14f4370c4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761112"
---
# <a name="domainstate-resource-type"></a>domainState 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在域中安排的异步操作的状态。

## <a name="properties"></a>属性

| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | 上次活动发生时的时间戳。 在计划操作、异步任务启动以及操作完成时，将更新该值。 |
| operation | String | 异步操作的类型。 值可以是 *ForceDelete 或* *Verification* |
| 状态 | String | 操作的当前状态。 <br> *计划* - 操作已计划，但尚未启动。 <br> *InProgress* - 任务已启动，正在进行中。 <br> *失败* - 操作失败。 |

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


