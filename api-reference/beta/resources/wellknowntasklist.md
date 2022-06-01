---
title: wellKnownTaskList 资源类型
description: 无法重命名或删除的内置任务列表。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0391983a88f91255779b994221fed195ad890c7e
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821195"
---
# <a name="wellknowntasklist-resource-type-deprecated"></a>wellKnownTaskList 资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

无法重命名或删除的内置任务列表。 微软待办有两个内置列表，**即标记的电子邮件** 和 **任务** 列表。

此资源支持将数据作为[开放扩展](/graph/extensibility-overview)添加到自定义属性

继承自 [baseTaskList](../resources/basetasklist.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 wellKnownTaskLists](../api/tasks-list-lists.md)|[wellKnownTaskList](../resources/wellknowntasklist.md) 集合|获取 [wellKnownTaskList](../resources/wellknowntasklist.md) 对象及其属性的列表。|
|[获取 wellKnownTaskList](../api/basetasklist-get.md)|[wellKnownTaskList](../resources/wellknowntasklist.md)|读取 [wellKnownTaskList](../resources/wellknowntasklist.md) 对象的属性和关系。|
|[List tasks](../api/basetasklist-list-tasks.md)|[baseTask](../resources/basetask.md) 集合|从任务导航属性获取 baseTask 资源。|
|[创建 baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|创建新的 baseTask 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|任务列表的名称。 继承自 [baseTaskList](../resources/basetasklist.md)。|
|id|String|任务列表的标识符，在用户的邮箱中是唯一的。 只读。 继承自 [baseTaskList](../resources/basetasklist.md)。|
|wellKnownListName|wellKnownListName_v2|如果给定列表是已知列表，则指示列表名称的属性。 可能的值包括 `none`、`defaultList`、`flaggedEmails`、`unknownFutureValue`。|

### <a name="wellknownlistname-values"></a>wellknownListName 值
|成员|说明|
|:---|:---|
|无| 用户创建的列表。|
|defaultList| 内置 **任务** 列表。|
|flaggedEmails| 内置 **标记的电子邮件** 列表。 此列表中包含来自已标记电子邮件的任务。|
|unknownFutureValue| 可变枚举 sentinel 值。 请勿使用。|

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
  "@odata.type": "microsoft.graph.wellKnownTaskList",
  "baseType": "microsoft.graph.baseTaskList",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.wellKnownTaskList",
  "displayName": "String",
  "id": "String (identifier)",
  "wellKnownListName": "String"
}
```

