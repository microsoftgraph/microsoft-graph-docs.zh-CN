---
title: outlookTaskGroup 资源类型
description: '一组文件夹 (outlookTaskFolder), 其中包含 Outlook 任务 (outlookTask 对象的集合)。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d519e18723ac9fbd38e7cec64a6758b0c9396bc2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966277"
---
# <a name="outlooktaskgroup-resource-type"></a>outlookTaskGroup 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一组文件夹 ([outlookTaskFolder](outlooktaskfolder.md)), 其中包含 Outlook 任务 ( [outlookTask](outlooktask.md)对象的集合)。 

在 Outlook 中, 有一个不能重`My Tasks`命名或删除的默认任务组。 不过, 您可以创建其他任务组。 


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 outlookTaskGroup](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |获取指定的 Outlook 任务组的属性和关系。|
|[创建 outlookTaskFolder](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| 创建一个 Outlook 任务文件夹。|
|[列出 taskFolders](../api/outlooktaskgroup-list-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)集合| 获取 Outlook 任务文件夹的集合。|
|[更新](../api/outlooktaskgroup-update.md) | [outlookTaskGroup](outlooktaskgroup.md)  |更新 Outlook 任务组的可写属性。 |
|[删除](../api/outlooktaskgroup-delete.md) | 无 |删除指定的 Outlook 任务组。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|changeKey|String|任务组的版本。|
|groupKey|Edm.Guid|任务组的唯一 GUID 标识符。|
|id|String|任务组的唯一字符串标识符。 只读。|
|isDefaultGroup|Boolean|如此如果任务组是默认任务组。|
|name|字符串|任务组的名称。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|taskFolders|[outlookTaskFolder](outlooktaskfolder.md)集合| 任务组中的任务文件夹的集合。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
