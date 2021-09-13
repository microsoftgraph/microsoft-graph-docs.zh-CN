---
title: todo 资源类型
description: 表示用户可以使用的微软待办服务。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ae754c758b3b1112c6201f4cbbbb143eb5af6d96
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128009"
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



