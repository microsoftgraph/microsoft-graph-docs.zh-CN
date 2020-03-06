---
title: plannerTaskDetails 资源类型
description: '**PlannerTaskDetails**资源表示有关任务的其他信息。 每个任务对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4dda174401ebf3435c7a190a3f92167ac6b47c0d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533977"
---
# <a name="plannertaskdetails-resource-type"></a>plannerTaskDetails 资源类型

命名空间：microsoft.graph

**PlannerTaskDetails**资源表示有关任务的其他信息。 每个[任务](plannertask.md)对象都有一个详细信息对象。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md) |读取**plannerTaskDetails**对象的属性和关系。|
|[更新](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md)    |更新**plannerTaskDetails**对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|任务上的检查表项目集合。|
|说明|字符串|任务描述|
|id|字符串| 只读。 任务详细信息的 ID。 长度为 28 个字符，区分大小写。 [格式验证](planner-identifiers-disclaimer.md)在服务上完成。|
|previewType|string|这将设置显示在任务上的预览类型。 可能的值包括 `automatic`、`noPreview`、`checklist`、`description`、`reference`。 将设置为`automatic`显示的预览由查看任务的应用程序选择。|
|references|[plannerExternalReferences](plannerexternalreferences.md)|任务上的引用集合。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
