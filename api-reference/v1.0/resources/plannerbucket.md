---
title: plannerBucket 资源类型
description: ) 中计划的任务Microsoft 365。 它包含在 plannerPlan 中，并且可以具有 plannerTasks 的集合。
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 46360d413f676e6420f28b94b5ba91ec9237e681
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129843"
---
# <a name="plannerbucket-resource-type"></a>plannerBucket 资源类型

命名空间：microsoft.graph

**plannerBucket** 资源表示 (计划中的任务) 或"自定义列"Microsoft 365。 它包含在 [plannerPlan 中](plannerplan.md) ，可以有 [plannerTasks 集合](plannertask.md)。



## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md) |读取 **plannerBucket 对象的属性和** 关系。|
|[List plannerTasks](../api/plannerbucket-list-tasks.md) |[plannerTask](plannertask.md) 集合| 获取 **plannerTask** 对象集合。|
|[Create](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md)   | 创建新的 **plannerBucket** 对象。 |
|[更新](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md)   |更新 **plannerBucket** 对象。 |
|[删除](../api/plannerbucket-delete.md) | 无 |删除 **plannerBucket** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 存储桶的 ID。 长度为 28 个字符，区分大小写。 [格式验证](planner-identifiers-disclaimer.md)在服务上完成。|
|name|String|存储桶的名称。|
|orderHint|String|用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。|
|planId|String|存储桶所属的计划 ID。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md) collection| 只读。 可为空。 存储桶中的任务集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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

