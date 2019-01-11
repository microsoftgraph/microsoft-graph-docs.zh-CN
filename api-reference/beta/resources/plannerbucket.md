---
title: plannerBucket 资源类型
description: ) 中的 Office 365 中的计划任务。 它包含在 plannerPlan，并且可以具有的 plannerTasks 集合。
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: 4868fb3925fa3ae94571d5cc93b0da12434b00dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808118"
---
# <a name="plannerbucket-resource-type"></a>plannerBucket 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**plannerBucket** 资源表示 Office 365 计划中的任务的存储桶（或“自定义列”）。它包含在 [plannerPlan](plannerplan.md) 之中，并且可能具有 [plannerTasks](plannertask.md) 集合。



## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md) |读取 **plannerBucket** 对象的属性和关系。|
|[List plannerTasks](../api/plannerbucket-list-tasks.md) |[plannerTask](plannertask.md) collection| 获取 **plannerTask** 对象集合。|
|[Create](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md)   | 新建 **plannerBucket** 对象。 |
|[Update](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md)   |更新 **plannerBucket** 对象。 |
|[Delete](../api/plannerbucket-delete.md) | 无 |删除 **plannerBucket** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 存储桶的 ID。 它是 28 字符长度和区分大小写。 服务上执行[格式验证](tasks-identifiers-disclaimer.md)。|
|name|String|存储桶的名称。|
|orderHint|String|用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。|
|planId|String|此存储桶所属的计划 ID。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md) collection| 只读。可为 NULL。存储桶中的任务集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
