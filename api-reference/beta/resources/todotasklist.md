---
title: todoTaskList 资源类型
description: Microsoft 中的一个列表，其中包含一个或多个 todoTask 资源。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0523404e836223f8a59e191d1e7040a279433795
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073381"
---
# <a name="todotasklist-resource-type"></a>todoTaskList 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft 中的一个列表，其中包含一个或多个 [todoTask](./todotask.md) 资源。 

在中，有一些内置的任务列表（如已 **标记的电子邮件** 和 **任务** ），无法重命名或删除。  不过，您可以创建其他任务列表。

此资源支持
* 将数据作为[开放扩展](/graph/extensibility-overview)添加到自定义属性
* 使用 [delta 查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出列表](../api/todo-list-lists.md) | [todoTaskList](todotasklist.md) 集合 | 获取用户邮箱中的所有 [todoTaskList](todotasklist.md) 。 |
|[创建 todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | 在用户的邮箱中创建 [todoTaskList](todotasklist.md) 。 |
|[获取任务列表](../api/todotasklist-get.md)|[todoTaskList](todotasklist.md)|读取指定 [todoTaskList](todotasklist.md)的属性和关系。|
|[更新任务列表](../api/todotasklist-update.md)|[todoTaskList](todotasklist.md)| 更新指定 [todoTaskList](todotasklist.md)的可写属性。|
|[删除任务列表](../api/todotasklist-delete.md)|无| 删除指定的 [todoTaskList](todotasklist.md) 。|
|[List tasks](../api/todotasklist-list-tasks.md)|[todoTask](todotask.md) 集合|获取指定列表中的所有 [todoTask](todotask.md) 资源。|
|[创建任务](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| 在指定的任务列表中创建 [todoTask](todotask.md) 。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|任务列表的名称。|
|id|String| 任务列表的标识符，在用户的邮箱中是唯一的。 只读。 继承自 [entity](entity.md)|
|isOwner|Boolean| 如果用户是给定任务列表的所有者，则为 True。|
|isShared|Boolean| 如果任务列表与其他用户共享，则为 True|
|wellknownListName|wellknownListName| 指示已知列表名称的属性（如果给定列表是已知列表）。 可取值为：`none`、`defaultList`、`flaggedEmails`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|extensions|[扩展](extension.md)集合| 为任务列表定义的开放扩展的集合。 可为 Null。|
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



