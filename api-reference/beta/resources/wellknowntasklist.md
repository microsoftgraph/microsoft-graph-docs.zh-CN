---
title: wellKnownTaskList 资源类型
description: 无法重命名或删除的内置任务列表。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0594ac7082680096ce17b3780780cc105e30606c
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424871"
---
# <a name="wellknowntasklist-resource-type"></a>wellKnownTaskList 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

无法重命名或删除的内置任务列表。 微软待办两个内置列表，**即已标记的电子邮件和****任务** 列表。

此资源支持将数据作为开放扩展添加到 [自定义属性](/graph/extensibility-overview)

继承自 [baseTaskList](../resources/basetasklist.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 wellKnownTaskLists](../api/tasks-list-lists.md)|[wellKnownTaskList](../resources/wellknowntasklist.md) 集合|获取 [wellKnownTaskList 对象](../resources/wellknowntasklist.md) 及其属性的列表。|
|[获取 wellKnownTaskList](../api/basetasklist-get.md)|[wellKnownTaskList](../resources/wellknowntasklist.md)|读取 [wellKnownTaskList 对象的属性和](../resources/wellknowntasklist.md) 关系。|
|[List tasks](../api/basetasklist-list-tasks.md)|[baseTask](../resources/basetask.md) 集合|从 tasks 导航属性获取 baseTask 资源。|
|[创建 baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|创建新的 baseTask 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|任务列表的名称。 继承自 [baseTaskList](../resources/basetasklist.md)。|
|id|字符串|任务列表的标识符，在用户邮箱中是唯一的。 只读。 继承自 [baseTaskList](../resources/basetasklist.md)。|
|wellKnownListName|wellKnownListName_v2|如果给定列表是已知列表，则指示列表名称的属性。 可能的值包括 `none`、`defaultList`、`flaggedEmails`、`unknownFutureValue`。|

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
|extensions|[扩展](../resources/extension.md)集合|为任务列表定义的开放扩展集合。 可为 NULL。 继承自 [baseTaskList](../resources/basetasklist.md)|
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

