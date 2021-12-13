---
title: 任务资源类型
description: 表示微软待办可用的任务服务
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a354c71449b5934ae0479eb1833258e394d6987e
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424877"
---
# <a name="tasks-resource-type"></a>任务资源类型

命名空间：microsoft.graph

表示微软待办可用的任务服务。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出列表](../api/tasks-list-lists.md)|[baseTaskList](../resources/basetasklist.md) 集合|从 lists 导航属性获取 baseTaskList 资源。|
|[创建 taskList](../api/tasks-post-lists.md)|[taskList](../resources/basetasklist.md)|创建新的 baseTaskList 对象。|

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|alltasks|[baseTask](../resources/basetask.md) 集合|用户邮箱中所有任务。|
|lists|[baseTaskList](../resources/basetasklist.md) 集合|用户邮箱中的任务列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tasks",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tasks",
  "id": "String (identifier)"
}
```

