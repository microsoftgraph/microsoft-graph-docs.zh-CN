---
title: plannerTask 资源类型
description: '**PlannerTask**资源表示 Microsoft 365 中的 Planner 任务。计划中包含规划器任务，可将其分配给计划中的存储桶。每个任务对象都有一个详细信息对象，该对象可包含有关任务的详细信息。有关组、计划和任务之间的关系的详细信息，请参阅概述。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b630976abce3ecebb92eed84ec593f9a1e70f2cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063994"
---
# <a name="plannertask-resource-type"></a>plannerTask 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerTask**资源表示 Microsoft 365 中的 Planner 任务。[计划](plannerplan.md)中包含规划器任务，可将其分配给计划中的[存储桶](plannerbucket.md)。每个任务对象都有一个[详细](plannertaskdetails.md)信息对象，该对象可包含有关任务的详细信息。有关组、计划和任务之间的关系的详细信息，请参阅[概述](planner-overview.md)。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerTask](../api/plannertask-get.md) | [plannerTask](plannertask.md) |读取 **plannerTask** 对象的属性和关系。|
|[更新](../api/plannertask-update.md) | [plannerTask](plannertask.md) |更新 **plannerTask** 对象。 |
|[删除](../api/plannertask-delete.md) | 无 |删除 **plannerTask** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|activeChecklistItemCount|Int32|核对清单项的数量，其值设置为 `false`，表示项目不全。|
|appliedCategories|[plannerAppliedCategories](plannerappliedcategories.md)|此任务已应用的类别。有关可能的值，请参阅[已应用的类别](plannerappliedcategories.md)。|
|assigneePriority|String|用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。|
|assignments|[plannerAssignments](plannerassignments.md)|被分配任务的接受者集合。|
|bucketId|String|此任务所属的存储桶 ID。 存储桶需要位于任务所在的计划中。 长度为 28 个字符，区分大小写。 [格式验证](tasks-identifiers-disclaimer.md)在服务上完成。 |
|checklistItemCount|Int32|任务上存在的核对清单项的数目。|
|completedBy|[identitySet](identityset.md)|完成任务的用户的身份。|
|completedDateTime|DateTimeOffset|只读。任务的 `'percentComplete'` 被设置为 `'100'` 的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|conversationThreadId|字符串|关于任务的对话的线程 ID。此为在组中创建的对话线程对象的 ID。|
|createdBy|[identitySet](identityset.md)|创建任务的用户的身份|
|createdDateTime|DateTimeOffset|只读。创建任务的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|dueDateTime|DateTimeOffset|任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|hasDescription|Boolean|只读。如果任务的 details 对象具有非空的说明，则值为 `true`，否则为 `false`。|
|id|String|只读。 任务的 ID。 长度为 28 个字符，区分大小写。 [格式验证](tasks-identifiers-disclaimer.md)在服务上完成。|
|orderHint|String|用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。|
|percentComplete|Int32|任务完成的百分比。当设置为 `100` 时，任务被视为完成。 |
|priority|Int32|任务的优先级。 值的有效范围介于 `0` 和 `10` (包含) 之间，且递增的值为低优先级 (`0` 具有最高优先级，并 `10` 具有最低优先级的) 。  目前，规划者将值 `0` 和 `1` "紧急"， `2` 以及 `3` `4` "重要"、、、、和 " `5` `6` `7` `8` `9` `10` 低" 的值解释为 "中"。  目前，规划器将设置 `1` "紧急"、" `3` 重要"、" `5` 中" 和 `9` "低" 的值。|
|planId|String|任务所属的计划 ID。|
|previewType|String|这将设置显示在任务上的预览类型。 可取值为：`automatic`、`noPreview`、`checklist`、`description`、`reference`。|
|referenceCount|Int32|任务上存在的外部引用的数量。|
|startDateTime|DateTimeOffset|任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|title|String|任务的标题。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)| 只读。可为 NULL。用于在按 assignedTo 分组时在任务板视图中正确呈现任务。|
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)| 只读。可为 NULL。用于在按存储桶分组时在任务板视图中正确呈现任务。|
|详细信息|[plannerTaskDetails](plannertaskdetails.md)| 只读。可为 NULL。关于任务的其他详细信息。|
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)| 只读。可为 NULL。用于在按进度分组时在任务板视图中正确呈现任务。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerTask"
}-->

```json
{
  "activeChecklistItemCount": 1024,
  "appliedCategories": {"@odata.type": "microsoft.graph.plannerAppliedCategories"},
  "assigneePriority": "String",
  "assignments": {"@odata.type": "microsoft.graph.plannerAssignments"},
  "bucketId": "String",
  "checklistItemCount": 1024,
  "completedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "id": "String (identifier)",
  "orderHint": "String",
  "percentComplete": 1024,
  "priority": 1024,
  "planId": "String",
  "previewType": "String",
  "referenceCount": 1024,
  "startDateTime": "String (timestamp)",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


