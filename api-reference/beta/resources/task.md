---
title: 任务资源类型
description: 表示可跟踪和完成的任务（如工作项或个人项）。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6d07d876535115c26b42d808e6870ec65f5dd2eb
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821237"
---
# <a name="task-resource-type-deprecated"></a>已弃用的任务资源类型 () 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

表示可跟踪和完成的任务（如工作项或个人项）。 **任务** 始终包含在 [基本任务列表](basetasklist.md)中。 

此资源支持以下各项：
* 在 [打开的扩展中](/graph/extensibility-overview)将数据添加为自定义属性。
* 订阅[更改通知](/graph/webhooks)。
* 使用 [增量查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。

继承自 [baseTask](../resources/basetask.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出任务](../api/basetasklist-list-tasks.md)|[任务](../resources/task.md)集合|获取 [任务](../resources/task.md) 对象及其属性的列表。|
|[获取任务](../api/basetask-get.md)|[任务](../resources/task.md)|读取 [任务](../resources/task.md) 对象的属性和关系。|
|[更新任务](../api/basetask-update.md)|[任务](../resources/task.md)|更新 [任务](../resources/task.md) 对象的属性。|
|[删除任务](../api/basetask-delete.md)|无|删除 [任务](../resources/task.md) 对象。|
|[移动](../api/basetask-move.md)|[baseTask](../resources/basetask.md)|将消息移动到其他列表。|
|[列出 checklistItems](../api/todotask-list-checklistitems.md)|[checklistItem](../resources/checklistitem.md) 集合|从 checklistItems 导航属性获取 checklistItem 资源。|
|[创建 checklistItem](../api/todotask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|创建新的 checklistItem 对象。|
|[列出 linkedResources](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) 集合|从 linkedResources 导航属性获取linkedResource_v2资源。|
|[创建 linkedResource](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|创建新的linkedResource_v2对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|textbody|[itemBody](../resources/itembody.md)|通常包含有关任务的信息的文本格式的任务正文。 继承自 [baseTask](../resources/basetask.md)。|
|bodyLastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。 继承自 [baseTask](../resources/basetask.md)。|
|completedDateTime|DateTimeOffset|任务完成的日期。 继承自 [baseTask](../resources/basetask.md)。|
|createdDateTime|DateTimeOffset|任务的创建日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。 继承自 [baseTask](../resources/basetask.md)。|
|displayName|String|任务的名称。 继承自 [baseTask](../resources/basetask.md)。|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内完成任务的日期。 继承自 [baseTask](../resources/basetask.md)。|
|id|String|任务的唯一标识符。 默认情况下，如果任务从一个列表移动到另一个列表，则此值不会更改。 继承自 [baseTask](../resources/basetask.md)。|
|importance|importance|任务的重要性。 可取值为：`low`、`normal`、`high`。 继承自 [baseTask](../resources/basetask.md)。 可能的值包括 `low`、`normal`、`high`。|
|lastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。 继承自 [baseTask](../resources/basetask.md)。|
|观点|[taskViewpoint](../resources/taskviewpoint.md)|用户的个人属性，例如 **reminderDateTime** 和 **类别**。 继承自 [baseTask](../resources/basetask.md)。|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|任务的定期模式。 继承自 [baseTask](../resources/basetask.md)。|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内开始执行任务的日期。 继承自 [baseTask](../resources/basetask.md)。|
|status|taskStatus_v2|指示任务的状态或进度。 可能的值为： `notStarted`， `inProgress`， `completed`，`unknownFutureValue`。 继承自 [baseTask](../resources/basetask.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|checklistItems|[checklistItem](../resources/checklistitem.md) 集合|链接到任务的 checklistItems 的集合。 继承自 [baseTask](../resources/basetask.md)|
|extensions|[扩展](../resources/extension.md)集合|为任务定义的开放扩展的集合。 继承自 [baseTask](../resources/basetask.md)|
|linkedResources|[linkedResource_v2](../resources/linkedresource_v2.md) 集合|链接到任务的资源集合。 继承自 [baseTask](../resources/basetask.md)|
|parentList|[baseTaskList](../resources/basetasklist.md)|包含任务的列表。 继承自 [baseTask](../resources/basetask.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.task",
  "baseType": "microsoft.graph.baseTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.task",
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

