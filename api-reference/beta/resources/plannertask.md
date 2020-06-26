---
title: plannerTask 资源类型
description: The **plannerTask** resource represents a Planner task in Microsoft 365. A Planner task is contained in a plan and can be assigned to a bucket in a plan. Each task object has a details object which can contain more information about the task. See overview for more information regarding relationships between group, plan and task.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 07374c6e8dc2dfaee1caba9f7283a1404627fb22
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897342"
---
# <a name="plannertask-resource-type"></a>plannerTask 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The **plannerTask** resource represents a Planner task in Microsoft 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.


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
|appliedCategories|[plannerAppliedCategories](plannerappliedcategories.md)|The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.|
|assigneePriority|String|Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).|
|assignments|[plannerAssignments](plannerassignments.md)|被分配任务的接受者集合。|
|bucketId|String|此任务所属的存储桶 ID。 存储桶需要位于任务所在的计划中。 长度为 28 个字符，区分大小写。 [格式验证](tasks-identifiers-disclaimer.md)在服务上完成。 |
|checklistItemCount|Int32|任务上存在的核对清单项的数目。|
|completedBy|[identitySet](identityset.md)|完成任务的用户的身份。|
|completedDateTime|DateTimeOffset|Read-only. Date and time at which the `'percentComplete'` of the task is set to `'100'`. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|conversationThreadId|字符串|Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.|
|createdBy|[identitySet](identityset.md)|创建任务的用户的身份|
|createdDateTime|DateTimeOffset|Read-only. Date and time at which the task is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|dueDateTime|DateTimeOffset|Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|hasDescription|Boolean|Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.|
|id|String|只读。 任务的 ID。 长度为 28 个字符，区分大小写。 [格式验证](tasks-identifiers-disclaimer.md)在服务上完成。|
|orderHint|String|Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).|
|percentComplete|Int32|Percentage of task completion. When set to `100`, the task is considered completed. |
|priority|Int32|任务的优先级。 值的有效范围介于 `0` 和 `10` （含）之间，并且值越低，优先级越低（ `0` 具有最高优先级， `10` 优先级最低）。  目前，规划者将值 `0` 和 `1` "紧急"， `2` 以及 `3` `4` "重要"、、、、和 " `5` `6` `7` `8` `9` `10` 低" 的值解释为 "中"。  目前，规划器将设置 `1` "紧急"、" `3` 重要"、" `5` 中" 和 `9` "低" 的值。|
|planId|String|任务所属的计划 ID。|
|previewType|String|这将设置显示在任务上的预览类型。 可取值为：`automatic`、`noPreview`、`checklist`、`description`、`reference`。|
|referenceCount|Int32|任务上存在的外部引用的数量。|
|startDateTime|DateTimeOffset|Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|title|String|任务的标题。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)| Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.|
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)| Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.|
|详细信息|[plannerTaskDetails](plannertaskdetails.md)| Read-only. Nullable. Additional details about the task.|
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)| Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.|

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
