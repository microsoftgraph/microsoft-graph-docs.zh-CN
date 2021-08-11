---
title: todoTaskList 资源类型
description: 包含一微软待办 todoTask 资源的列表。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7e0b51647ed53a7e1f7500f3322c840f7476218f0c99888de7c700fb36c4820e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124008"
---
# <a name="todotasklist-resource-type"></a>todoTaskList 资源类型

命名空间：microsoft.graph

包含一微软待办[todoTask](./todotask.md)资源的列表。 

在微软待办中，内置任务列表（如已标记的电子邮件和 **任务**）无法重命名或删除。   但是，您可以创建其他任务列表。

此资源支持
* 将数据作为开放扩展添加到 [自定义属性](/graph/extensibility-overview)
* 使用 [增量查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出列表](../api/todo-list-lists.md) | [todoTaskList](todotasklist.md) 集合 | 获取用户邮箱中所有的[todoTaskList。](todotasklist.md) |
|[创建 todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | 在[用户邮箱中创建 todoTaskList。](todotasklist.md) |
|[获取任务列表](../api/todotasklist-get.md)|[todoTaskList](todotasklist.md)|读取指定的 [todoTaskList 的属性和关系](todotasklist.md)。|
|[更新任务列表](../api/todotasklist-update.md)|[todoTaskList](todotasklist.md)| 更新指定 [todoTaskList 的可写属性](todotasklist.md)。|
|[删除任务列表](../api/todotasklist-delete.md)|无| 删除指定的 [todoTaskList](todotasklist.md) 。|
|[列出任务](../api/todotasklist-list-tasks.md)|[todoTask](todotask.md) 集合|获取指定列表中的所有 [todoTask](todotask.md) 资源。|
|[创建任务](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| 在指定的任务列表中创建 [todoTask](todotask.md)。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|任务列表的名称。|
|id|String| 任务列表的标识符，在用户邮箱中是唯一的。 只读。 继承自 [实体](entity.md)|
|isOwner|Boolean| 如果用户是给定任务列表的所有者，则其为 True。|
|isShared|Boolean| 如此 如果任务列表与其他用户共享|
|wellknownListName|wellknownListName| 如果给定列表是已知列表，则指示列表名称的属性。 可取值为：`none`、`defaultList`、`flaggedEmails`、`unknownFutureValue`。|

### <a name="wellknownlistname-values"></a>wellknownListName 值
|成员|说明|
|:---|:---|
|无| 用户创建的列表。|
|defaultList| 内置 **任务列表** 。|
|flaggedEmails| 内置的已 **标记电子邮件** 列表。 此列表中存在来自已标记电子邮件的任务。|
|unknownFutureValue| 可发展枚举 sentinel 值。 请勿使用。|

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



