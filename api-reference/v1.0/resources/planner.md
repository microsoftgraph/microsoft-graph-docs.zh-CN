---
title: planner 资源类型
description: 规划 **器** 资源是 Planner 对象模型的入口点。 它返回一个单一 **规划器** 资源。  它不包含任何可用属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8fc5f91dd8da85b259dd792a0926311d57098ee9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470674"
---
# <a name="planner-resource-type"></a>planner 资源类型

命名空间：microsoft.graph

规划 **器** 资源是 Planner 对象模型的入口点。 它返回一个单一 **规划器** 资源。  它不包含任何可用属性。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| 通过发布到存储桶集合创建新的 **plannerBucket。**|
|[创建 plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| 通过发布到 **计划集合创建新的 plannerPlan。**|
|[创建 plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| 通过发布到 **任务集合创建新的 plannerTask。**|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) collection| 只读。 可为 NULL。 返回指定存储桶的集合|
|计划|[plannerPlan](plannerplan.md) 集合| 只读。 可为 NULL。 返回指定计划的集合|
|tasks|[plannerTask](plannertask.md) collection| 只读。 可为 NULL。 返回指定任务的集合|

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

**规划器** 资源位于图形的根目录下。

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
```http
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

