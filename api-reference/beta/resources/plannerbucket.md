---
title: plannerBucket 资源类型
description: ) 用于 Office 365 中的计划中的任务。 它包含在 plannerPlan 中, 并且可以具有 plannerTasks 的集合。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 85cf30bc13b3236928e662807a144f81614adbd7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579252"
---
# <a name="plannerbucket-resource-type"></a>plannerBucket 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerBucket**资源表示 Office 365 中的计划中的任务的存储桶 (或 "自定义列")。 它包含在[plannerPlan](plannerplan.md)中, 并且可以具有[plannerTasks](plannertask.md)的集合。



## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md) |读取**plannerBucket**对象的属性和关系。|
|[List plannerTasks](../api/plannerbucket-list-tasks.md) |[plannerTask](plannertask.md) 集合| 获取**plannerTask**对象集合。|
|[创建](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md)   | 创建新的**plannerBucket**对象。 |
|[更新](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md)   |更新**plannerBucket**对象。 |
|[删除](../api/plannerbucket-delete.md) | 无 |删除**plannerBucket**对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 存储桶的 ID。 长度为 28 个字符，区分大小写。 [格式验证](tasks-identifiers-disclaimer.md)在服务上完成。|
|name|String|存储桶的名称。|
|orderHint|String|用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。|
|planId|String|存储桶所属的计划 ID。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|任务|[plannerTask](plannertask.md) 集合| 只读。 可为 Null。 存储桶中的任务的集合。|

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerbucket.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
