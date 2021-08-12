---
title: todo 资源类型
description: 表示用户可以使用的微软待办服务。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 89bbdd1bd3d91c5114850ffad8afc3aeec90e8bf3bbfb0b65e540444c2022b7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235259"
---
# <a name="todo-resource-type"></a>todo 资源类型

命名空间：microsoft.graph

表示用户可以使用的微软待办服务。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出列表](../api/todo-list-lists.md) | [todoTaskList](todotasklist.md) 集合 | 获取用户邮箱中的所有任务列表。 |
|[创建 todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | 在用户的邮箱中创建微软待办任务列表。 |

## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|lists|[todoTaskList](../resources/todotasklist.md) 集合| 用户邮箱中的任务列表。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todo",
  "id": "String"
}
```



