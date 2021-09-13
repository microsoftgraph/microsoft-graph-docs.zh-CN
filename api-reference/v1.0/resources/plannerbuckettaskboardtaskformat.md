---
title: plannerBucketTaskBoardTaskFormat 资源类型
description: '**plannerBucketTaskBoardTaskFormat** 资源表示用于在任务板的存储桶视图中正确呈现任务的信息 (该视图按分配给) 的存储桶中的任务组织。 每个任务都有一个 **与之关联的 plannerBucketTaskBoardTaskFormat** 对象。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 809622d656a56b4f21c0660515602ab468c1f5e7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044319"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a>plannerBucketTaskBoardTaskFormat 资源类型

命名空间：microsoft.graph

**plannerBucketTaskBoardTaskFormat** 资源表示用于在任务板的存储桶视图中正确呈现任务的信息 (该视图按分配给) 的存储桶中的任务组织。 每个 [任务](plannertask.md) 都有一个 **与之关联的 plannerBucketTaskBoardTaskFormat** 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) |读取 **plannerBucketTaskBoardTaskFormat 对象的属性和** 关系。|
|[更新](../api/plannerbuckettaskboardtaskformat-update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)  |更新 **plannerBucketTaskBoardTaskFormat** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 资源的 ID。 长度为 28 个字符，区分大小写。 [格式验证](planner-identifiers-disclaimer.md)在服务上完成。|
|orderHint|String|用于为任务板存储桶视图中的任务进行排序的提示。[此处](planner-order-hint-format.md)概述了此格式。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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

