---
title: todoTaskList 资源类型
description: Microsoft To Do 中的一个或多个 todoTask 资源的列表。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d34f90329fc6ca4d5e12ff2f2b191819b88f895b
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849869"
---
# <a name="todotasklist-resource-type"></a>todoTaskList 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft To Do 中的一个或多个 [todoTask 资源](./todotask.md) 的列表。 

In To Do， there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.  但是，你可以创建其他任务列表。

该资源支持
* 将数据作为开放扩展添加到 [自定义属性](/graph/extensibility-overview)
* 使用 [delta 查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表列表](../api/todo-list-lists.md) | [todoTaskList](todotasklist.md) 集合 | 获取用户[邮箱中的所有 todoTaskList。](todotasklist.md) |
|[创建 todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | 在[用户邮箱中创建 todoTaskList。](todotasklist.md) |
|[获取任务列表](../api/todotasklist-get.md)|[todoTaskList](todotasklist.md)|读取指定的 [todoTaskList 的属性和关系](todotasklist.md)。|
|[更新任务列表](../api/todotasklist-update.md)|[todoTaskList](todotasklist.md)| 更新指定的 [todoTaskList 的可写属性](todotasklist.md)。|
|[删除任务列表](../api/todotasklist-delete.md)|无| 删除指定的 [todoTaskList](todotasklist.md) 。|
|[List tasks](../api/todotasklist-list-tasks.md)|[todoTask](todotask.md) 集合|获取指定 [列表中的所有 todoTask](todotask.md) 资源。|
|[创建任务](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| 在指定[任务列表中创建 todoTask。](todotask.md)|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|任务列表的名称。|
|id|String| 任务列表的标识符，在用户邮箱中是唯一的。 只读。 从实体 [继承](entity.md)|
|isOwner|Boolean| 如果用户是给定的任务列表的所有者，则为 True 。|
|isShared|Boolean| 如此 如果任务列表与其他用户共享|
|wellknownListName|wellknownListName| 指示给定列表是否是已知列表的已知列表名称的属性。 可取值为：`none`、`defaultList`、`flaggedEmails`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|extensions|[扩展](extension.md)集合| 为任务列表定义的开放扩展集合。 可为 Null。|
|任务|[todoTask](todotask.md) 集合|此任务列表中的任务。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTaskList",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "String (identifier)",
  "displayName": "String",
  "isOwner": "Boolean",
  "isShared": "Boolean",
  "wellknownListName": "String"
}
```

