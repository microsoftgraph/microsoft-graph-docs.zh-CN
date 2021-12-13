---
title: taskList 资源类型
description: 表示用户在包含一个或多个任务微软待办中创建的列表。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 070a427de0531e5ce715e31c91b2ffddd6be4576
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424881"
---
# <a name="tasklist-resource-type"></a>taskList 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户在包含一个或多个任务微软待办[中创建的列表。](./task.md) 

此资源支持
* 将数据作为开放扩展添加到 [自定义属性](/graph/extensibility-overview)
* 使用 [delta 查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。

继承自 [baseTaskList](../resources/basetasklist.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 taskLists](../api/tasks-list-lists.md)|[taskList](../resources/tasklist.md) 集合|获取 [taskList 对象](../resources/tasklist.md) 及其属性的列表。|
|[获取 taskList](../api/basetasklist-get.md)|[taskList](../resources/tasklist.md)|读取 [taskList 对象的属性和](../resources/tasklist.md) 关系。|
|[更新 taskList](../api/tasklist-update.md)|[taskList](../resources/tasklist.md)|更新 [taskList 对象](../resources/tasklist.md) 的属性。|
|[删除 taskList](../api/tasklist-delete.md)|无|删除 [taskList](../resources/tasklist.md) 对象。|
|[List tasks](../api/basetasklist-list-tasks.md)|[baseTask](../resources/basetask.md) 集合|从 tasks 导航属性获取 baseTask 资源。|
|[创建 baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|创建新的 baseTask 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|任务列表的名称。 继承自 [baseTaskList](../resources/basetasklist.md)。|
|id|字符串|任务列表的标识符，在用户邮箱中是唯一的。 只读。 继承自 [baseTaskList](../resources/basetasklist.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|extensions|[扩展](../resources/extension.md)集合|为任务列表定义的开放扩展集合。 可为 NULL。 继承自 [baseTaskList](../resources/basetasklist.md)|
|tasks|[baseTask](../resources/basetask.md) 集合|此任务列表中的任务。 只读。 可为 NULL。 继承自 [baseTaskList](../resources/basetasklist.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.taskList",
  "baseType": "microsoft.graph.baseTaskList",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taskList",
  "displayName": "String",
  "id": "String (identifier)"
}
```

