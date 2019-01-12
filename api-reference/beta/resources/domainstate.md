---
title: domainState 资源类型
description: 表示域上经过计划的异步操作的状态。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cee5ef9e0d0f4a5ada0d9117f755c407d081461d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963099"
---
# <a name="domainstate-resource-type"></a>domainState 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
