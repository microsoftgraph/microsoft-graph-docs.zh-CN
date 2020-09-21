---
title: planner 资源类型
description: '**Planner**资源是 planner 对象模型的入口点。 它返回单一实例 **planner** 资源。  它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f8333596ee93a42db8eded49815059e8633bf3db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037631"
---
# <a name="planner-resource-type"></a>planner 资源类型

命名空间：microsoft.graph

**Planner**资源是 planner 对象模型的入口点。 它返回单一实例 **planner** 资源。  它不包含任何可用属性。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| 通过发布到存储桶集合创建新的 **plannerBucket** 。|
|[创建 plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| 通过发布到计划集合创建新的 **plannerPlan** 。|
|[创建 plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| 通过发布到 tasks 集合创建新的 **plannerTask** 。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) collection| 只读。 可为 Null。 返回指定的存储桶的集合|
|计划|[plannerPlan](plannerplan.md) 集合| 只读。 可为 Null。 返回指定计划的集合|
|tasks|[plannerTask](plannertask.md) collection| 只读。 可为 Null。 返回指定任务的集合|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a>示例

**Planner**资源在图形的根目录中可用。

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

