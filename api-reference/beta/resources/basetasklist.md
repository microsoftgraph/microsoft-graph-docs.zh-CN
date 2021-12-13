---
title: baseTaskList 资源类型
description: 包含一个或多个任务资源。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7a0774bf6d51eba2bc55f67c58c2d7de5a0c3312
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424862"
---
# <a name="basetasklist-resource-type"></a>baseTaskList 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含一个或多个 [任务](./basetask.md) 资源。

这是以下派生类型的任务列表的基本资源。
* 内置任务列表 ([wellKnownTaskList](../resources/wellknowntasklist.md)) 
* 用户创建的任务列表 ([taskList](../resources/tasklist.md) 资源)  

这是一个抽象类型。

## <a name="methods"></a>方法
以下方法适用于任何派生类型的 **baseTaskList** (**wellKnownTaskList****、taskList**) 

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 baseTaskLists](../api/tasks-list-lists.md)|[baseTaskList](../resources/basetasklist.md) 集合|获取 [baseTaskList](../resources/basetasklist.md) 对象及其属性的列表。|
|[获取 baseTaskList](../api/basetasklist-get.md)|[baseTaskList](../resources/basetasklist.md)|读取 [baseTaskList 对象的属性和](../resources/basetasklist.md) 关系。|
|[List tasks](../api/basetasklist-list-tasks.md)|[baseTask](../resources/basetask.md) 集合|从 tasks 导航属性获取 baseTask 资源。|
|[创建 baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|创建新的 baseTask 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|任务列表的名称。|
|id|字符串|任务列表的标识符，在用户邮箱中是唯一的。 只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|extensions|[扩展](../resources/extension.md)集合|为任务列表定义的开放扩展集合。 可为 Null。|
|任务|[baseTask](../resources/basetask.md) 集合|此任务列表中的任务。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseTaskList",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.baseTaskList",
  "displayName": "String",
  "id": "String (identifier)"
}
```

