---
title: plannerBucketTaskBoardTaskFormat 资源类型
description: '**PlannerBucketTaskBoardTaskFormat**资源表示用于在任务板的 bucket 视图（按其分配的存储桶中的任务组织的视图）中正确呈现任务的信息。 每个任务都有一个与之关联的**plannerBucketTaskBoardTaskFormat**对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6815209c4a87ee348cb3c37f5b318a5022e4c5b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521781"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a>plannerBucketTaskBoardTaskFormat 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerBucketTaskBoardTaskFormat**资源表示用于在任务板的 bucket 视图（按其分配的存储桶中的任务组织的视图）中正确呈现任务的信息。 每个[任务](plannertask.md)都有一个与之关联的**plannerBucketTaskBoardTaskFormat**对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) |读取**plannerBucketTaskBoardTaskFormat**对象的属性和关系。|
|[更新](../api/plannerbuckettaskboardtaskformat-update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)  |更新**plannerBucketTaskBoardTaskFormat**对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|字符串| 只读。 资源的 ID。 长度为 28 个字符，区分大小写。 [格式验证](tasks-identifiers-disclaimer.md)在服务上完成。|
|orderHint|String|用于为任务板存储桶视图中的任务进行排序的提示。[此处](planner-order-hint-format.md)概述了此格式。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
