---
title: checklistItem 资源类型
description: 表示任务上的清单项的集合
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 804a245b25a8322cf7879dd2fb16f5575da22dc3
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821048"
---
# <a name="checklistitem-resource-type"></a>checklistItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi-sharedfeature](../includes/todo-deprecate-basetaskapi-sharedfeature.md)]

表示更大的 [todoTask](./todotask.md) 中的子任务。 **ChecklistItem** 允许将复杂任务分解为更可操作、更小的任务。 

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 checklistItems](../api/todotask-list-checklistitems.md)|[checklistItem](../resources/checklistitem.md) 集合|获取 [checklistItem](../resources/checklistitem.md) 对象及其与指定 [todoTask](./todotask.md) 关联的属性的列表。|
|[创建 checklistItem](../api/todotask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|创建与指定 [todoTask](./todotask.md) 关联的新 [checklistItem](../resources/checklistitem.md) 对象。|
|列出已弃用)  ([checklistItems](../api/basetask-list-checklistitems.md)|[checklistItem](../resources/checklistitem.md) 集合|获取 [checklistItem](../resources/checklistitem.md) 对象及其与指定 [baseTask](./basetask.md) 关联的属性的列表。|
|创建已弃用的 [checklistItem](../api/basetask-post-checklistitems.md) () |[checklistItem](../resources/checklistitem.md)|创建与指定 [baseTask](./basetask.md) 关联的新 [checklistItem](../resources/checklistitem.md) 对象。|
|[获取 checklistItem](../api/checklistitem-get.md)|[checklistItem](../resources/checklistitem.md)|读取 [checklistItem](../resources/checklistitem.md) 对象的属性和关系。|
|[更新 checklistItem](../api/checklistitem-update.md)|[checklistItem](../resources/checklistitem.md)|更新 [checklistItem](../resources/checklistitem.md) 对象的属性。|
|[删除 checklistItem](../api/checklistitem-delete.md)|无|删除 [checklistItem](../resources/checklistitem.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|checkedDateTime|DateTimeOffset|**checklistItem** 完成的日期和时间。|
|createdDateTime|DateTimeOffset|创建 **checklistItem** 的日期和时间。|
|displayName|String|指示 **checklistItem** 标题的字段。|
|id|String|**checkListItem** 的服务器生成的 ID|
|isChecked|布尔|指示是否签出项的状态。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.checklistItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.checklistItem",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "checkedDateTime": "String (timestamp)",
  "isChecked": "Boolean",
  "id": "String (identifier)"
}
```

