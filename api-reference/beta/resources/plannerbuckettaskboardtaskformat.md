---
title: plannerBucketTaskBoardTaskFormat 资源类型
description: '**plannerBucketTaskBoardTaskFormat** 资源表示用于在“任务板”的“存储桶”视图（由被分配到的存储桶中的任务组成的视图）下正确呈现任务的信息。每个任务均将有一个与其相关联的 **plannerBucketTaskBoardTaskFormat** 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ea557bad20aa0fd10a73e71902b959913e8fff12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986192"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a>plannerBucketTaskBoardTaskFormat 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**plannerBucketTaskBoardTaskFormat** 资源表示用于在“任务板”的“存储桶”视图（由被分配到的存储桶中的任务组成的视图）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerBucketTaskBoardTaskFormat** 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) |读取 **plannerBucketTaskBoardTaskFormat** 对象的属性和关系。|
|[Update](../api/plannerbuckettaskboardtaskformat-update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)  |更新 **plannerBucketTaskBoardTaskFormat** 对象 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 资源的 ID。 它是 28 字符长度和区分大小写。 服务上执行[格式验证](tasks-identifiers-disclaimer.md)。|
|orderHint|String|用于对任务板存储桶视图中的任务进行排序的提示。[此处](planner-order-hint-format.md)概述了此格式。|

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
