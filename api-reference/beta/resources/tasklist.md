---
title: taskList 资源类型
description: 表示用户在微软待办中创建的包含一个或多个任务资源的列表。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bee831640d6ba392f359a1ad1dbd70b088733141
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819355"
---
# <a name="tasklist-resource-type-deprecated"></a>已弃用的 taskList 资源类型 () 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

表示用户在微软待办中创建的包含一个或多个[任务资源的](./task.md)列表。 

此资源支持以下各项：
* 将数据作为[打开的扩展](/graph/extensibility-overview)添加到自定义属性
* 使用 [增量查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。

**taskList** 资源继承自 [baseTaskList](../resources/basetasklist.md)。
其内容（ **任务** 资源类型的内容）继承自 [baseTask](../resources/basetask.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 taskLists](../api/tasks-list-lists.md)|[taskList](../resources/tasklist.md) 集合|获取 [taskList](../resources/tasklist.md) 对象及其属性的列表。|
|[获取 taskList](../api/basetasklist-get.md)|[taskList](../resources/tasklist.md)|读取 [taskList](../resources/tasklist.md) 对象的属性和关系。|
|[更新 taskList](../api/tasklist-update.md)|[taskList](../resources/tasklist.md)|更新 [taskList](../resources/tasklist.md) 对象的属性。|
|[删除 taskList](../api/tasklist-delete.md)|无|删除 [taskList](../resources/tasklist.md) 对象。|
|[List tasks](../api/basetasklist-list-tasks.md)|[baseTask](../resources/basetask.md) 集合|从任务导航属性获取 baseTask 资源。|
|[创建 baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|创建新的 baseTask 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|任务列表的名称。 继承自 [baseTaskList](../resources/basetasklist.md)。|
|id|String|任务列表的标识符，在用户的邮箱中是唯一的。 只读。 继承自 [baseTaskList](../resources/basetasklist.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|extensions|[扩展](../resources/extension.md)集合|为任务列表定义的开放扩展的集合。 可为 NULL。 继承自 [baseTaskList](../resources/basetasklist.md)|
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

