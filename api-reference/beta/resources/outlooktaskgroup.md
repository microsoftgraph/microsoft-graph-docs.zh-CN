---
title: outlookTaskGroup 资源类型
description: '包含 Outlook 任务 （outlookTask 对象的集合） 的文件夹 (outlookTaskFolder) 组。 '
author: angelgolfer-ms
ms.openlocfilehash: 9fed69e1401f2b11ae3630a3c4cef66fd9446920
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359393"
---
# <a name="outlooktaskgroup-resource-type"></a>outlookTaskGroup 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

包含 Outlook 任务 （ [outlookTask](outlooktask.md)对象的集合） 的文件夹 ([outlookTaskFolder](outlooktaskfolder.md)) 组。 

在 Outlook 中，没有默认任务组`My Tasks`无法重命名或删除。 但是，您可以创建其他任务组。 


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 outlookTaskGroup](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |要获取的属性和指定 Outlook 任务组的关系。|
|[创建 outlookTaskFolder](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| 创建 Outlook 任务文件夹。|
|[列表 taskFolders](../api/outlooktaskgroup-list-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)集合| 获取 Outlook 任务文件夹的集合。|
|[Update](../api/outlooktaskgroup-update.md) | [outlookTaskGroup](outlooktaskgroup.md)  |更新 Outlook 任务组的可写属性。 |
|[删除](../api/outlooktaskgroup-delete.md) | 无 |删除指定的 Outlook 任务组。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|changeKey|字符串|任务组的版本。|
|groupKey|Edm.Guid|任务组的唯一 GUID 标识符。|
|id|字符串|任务组的唯一字符串标识符。 只读。|
|isDefaultGroup|Boolean|如果任务组的默认任务组，则为 true。|
|name|字符串|任务组的名称。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|taskFolders|[outlookTaskFolder](outlooktaskfolder.md)集合| 在任务组中的任务文件夹的集合。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->