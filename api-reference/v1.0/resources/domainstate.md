---
title: domainState 资源类型
description: 表示在域中安排的异步操作的状态。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3d2140d0b0067ec576433b442446472d0a6af80fd4152131ea79d384a8d623c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218798"
---
# <a name="domainstate-resource-type"></a>domainState 资源类型

命名空间：microsoft.graph

表示在域中安排的异步操作的状态。

## <a name="properties"></a>属性

| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | 上次活动发生时的时间戳。 在计划操作、异步任务启动以及操作完成时，将更新该值。 |
| operation | String | 异步操作的类型。 值可以是 *ForceDelete 或* *Verification* |
| status | String | 操作的当前状态。 <br> *计划* - 操作已计划，但尚未启动。 <br> *InProgress* - 任务已启动，正在进行中。 <br> *失败* - 操作失败。 |

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

