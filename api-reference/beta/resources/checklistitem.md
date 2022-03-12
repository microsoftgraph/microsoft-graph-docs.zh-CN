---
title: checklistItem 资源类型
description: 表示任务上检查表项的集合
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 86ec25ee83ae6cd1f30bf8a84b6177f870d39586
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451132"
---
# <a name="checklistitem-resource-type"></a>checklistItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表较大 [baseTask 中的子任务](./baseTask.md)。 **ChecklistItem** 允许将复杂的任务分解为更可操作、更小的任务。 

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 checklistItems](../api/basetask-list-checklistitems.md)|[checklistItem](../resources/checklistitem.md) 集合|获取 [checklistItem 对象](../resources/checklistitem.md) 及其属性的列表。|
|[创建 checklistItem](../api/basetask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|创建新的 [checklistItem](../resources/checklistitem.md) 对象。|
|[获取 checklistItem](../api/checklistitem-get.md)|[checklistItem](../resources/checklistitem.md)|读取 [checklistItem](../resources/checklistitem.md) 对象的属性和关系。|
|[更新 checklistItem](../api/checklistitem-update.md)|[checklistItem](../resources/checklistitem.md)|更新 [checklistItem 对象](../resources/checklistitem.md) 的属性。|
|[删除 checklistItem](../api/checklistitem-delete.md)|无|删除 [checklistItem](../resources/checklistitem.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|checkedDateTime|DateTimeOffset|完成 **checklistItem 的** 日期和时间。|
|createdDateTime|DateTimeOffset|创建 **checklistItem 的** 日期和时间。|
|displayName|字符串|指示 **checklistItem 标题的字段**。|
|id|字符串|**checkListItem 的服务器生成的 ID**|
|isChecked|布尔值|指示项目是否已签出的状态。|

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

