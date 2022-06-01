---
title: baseTask 资源类型
description: 表示可跟踪和完成的任务（如工作项或个人项）
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4ec4f4fd5f124f475a2183f468063051e4c26526
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820943"
---
# <a name="basetask-resource-type-deprecated"></a>已弃用的 baseTask 资源类型 () 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

一种抽象类型，表示可跟踪和完成的任务（如工作项或个人项）。

这是 [任务](task.md) 资源继承的基础类型。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 baseTasks](../api/basetasklist-list-tasks.md)|[baseTask](../resources/basetask.md) 集合|获取 [baseTask](../resources/basetask.md) 对象及其属性的列表。|
|[创建 baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|创建新的 [baseTask](../resources/basetask.md) 对象。|
|[获取 baseTask](../api/basetask-get.md)|[baseTask](../resources/basetask.md)|读取 [baseTask](../resources/basetask.md) 对象的属性和关系。|
|[更新 baseTask](../api/basetask-update.md)|[baseTask](../resources/basetask.md)|更新 [baseTask](../resources/basetask.md) 对象的属性。|
|[删除 baseTask](../api/basetask-delete.md)|无|删除 [baseTask](../resources/basetask.md) 对象。|
|[移动](../api/basetask-move.md)|[baseTask](../resources/basetask.md)|将消息移动到其他列表。|
|[delta](../api/basetask-delta.md)|[baseTask](../resources/basetask.md) 集合|获取一组已在指定列表中添加、删除或更新的 **baseTask** 对象。|
|[列出 checklistItems](../api/todotask-list-checklistitems.md)|[checklistItem](../resources/checklistitem.md) 集合|从 **checklistItems 导航属性获取 checklistItem** 资源。|
|[创建 checklistItem](../api/todotask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|创建新的 **checklistItem** 对象。|
|[列出 linkedResources](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) 集合|从 linkedResources 导航属性获取 **linkedResource_v2** 资源。|
|[创建linkedResource_v2](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|创建新的 **linkedResource_v2** 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|textBody|String|通常包含有关任务的信息的文本格式的任务正文。 |
|bodyLastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。 |
|completedDateTime|DateTimeOffset|任务完成的日期。 |
|createdDateTime|DateTimeOffset|任务的创建日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。 |
|displayName|String|任务的名称。 |
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内完成任务的日期。 |
|id|String|任务的唯一标识符。 默认情况下，如果任务从一个列表移动到另一个列表，则此值不会更改。 |
|importance|importance|任务的重要性。 可取值为：`low`、`normal`、`high`。  可能的值包括 `low`、`normal`、`high`。|
|lastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。 |
|观点|[taskViewpoint](../resources/taskviewpoint.md)|用户的个人属性，例如 **reminderDateTime** 和 **类别**。 |
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|任务的定期模式。 |
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内开始执行任务的日期。 |
|状态|taskStatus_v2|指示任务的状态或进度。 可能的值为： `notStarted`， `inProgress`， `completed`，`unknownFutureValue`。 |

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|checklistItems|[checklistItem](../resources/checklistitem.md) 集合|链接到更复杂的父任务的较小子任务的集合。 |
|extensions|[扩展](../resources/extension.md)集合|为任务定义的开放扩展的集合。 |
|linkedResources|[linkedResource_v2](../resources/linkedresource_v2.md) 集合|链接到任务的资源集合。 |
|parentList|[baseTaskList](../resources/basetasklist.md)|包含任务的列表。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.baseTask",
  "textBody": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "bodyLastModifiedDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "displayName": "String",
  "status": "String",
  "viewpoint": {
    "@odata.type": "microsoft.graph.taskViewpoint"
  },
  "id": "String (identifier)"
}
```

