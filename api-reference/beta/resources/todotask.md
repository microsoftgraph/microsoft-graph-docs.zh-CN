---
title: todoTask 资源类型
description: TodoTask 资源跟踪工作项。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 58859f2781ecec713e547340606411302232ec06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003491"
---
# <a name="todotask-resource-type"></a>todoTask 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TodoTask**表示可以跟踪和完成的任务，例如，一段工作或个人项目。 

**TodoTask**始终包含在[todoTaskList](todotasklist.md)中。 它包括与 [linkedResource](./linkedResource.md) 对象集合的关系，并跟踪任务的一个或多个源。

此资源支持以下内容：
* 在 [开放扩展](/graph/extensibility-overview)中将数据添加为自定义属性。
* 使用 [delta 查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List tasks](../api/todotasklist-list-tasks.md)|[todoTask](todotask.md) 集合|获取指定列表中的所有 [todoTask](todotask.md) 资源。|
|[创建任务](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| 在指定的任务列表中创建[todoTask](todotask.md)|
|[获取任务](../api/todotask-get.md)|[todoTask](../resources/todotask.md)|读取 [todoTask](../resources/todotask.md) 对象的属性和关系。|
|[更新任务](../api/todotask-update.md)|[todoTask](../resources/todotask.md)|更新 [todoTask](../resources/todotask.md) 对象的属性。|
|[删除任务](../api/todotask-delete.md)|无|删除一个 [todoTask](../resources/todotask.md) 对象。|
|[列出 linkedResources](../api/todotask-list-linkedresources.md)|[linkedResource](../resources/linkedresource.md) 集合|从 linkedResources 导航属性中获取 linkedResources。|
|[创建 linkedResources](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|创建新的 linkedResources 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|正文|[itemBody](../resources/itembody.md)|通常包含有关任务的信息的任务正文。|
|bodyLastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|在指定时区内完成任务的日期。|
|createdDateTime|DateTimeOffset|任务的创建日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式。 例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内完成任务的日期。|
|id|String|任务的唯一标识符。 默认情况下，在将项目从一个列表移动到另一个列表时，此值会发生更改。|
|importance|importance|任务的重要性。 可取值为：`low`、`normal`、`high`。|
|isReminderOn|Boolean|如果设置警报以提醒用户有任务，则设置为 true。|
|lastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。|
|定期|[patternedRecurrence](../resources/patternedrecurrence.md)|任务的定期模式。|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|提醒警报发出任务发生提醒的日期和时间。|
|状态|taskStatus|指示任务的状态或进度。 可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。|
|title|String|任务的简短说明。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|extensions|[扩展](extension.md)集合| 为任务定义的开放扩展的集合。 可为 Null。|
|linkedResources|[linkedResource](../resources/linkedresource.md) 集合|链接到任务的资源的集合。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTask",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTask",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "isReminderOn": "Boolean",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "reminderDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "status": "String",
  "title": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "bodyLastModifiedDateTime": "String (timestamp)"
}
```



