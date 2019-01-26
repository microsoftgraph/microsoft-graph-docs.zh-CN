---
title: outlookTaskFolder 资源类型
description: '包含 Outlook 任务 （outlookTask 对象的集合） 的文件夹。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a117e14ea1cfe4b69cbbf69720a22a0094fb0b72
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575665"
---
# <a name="outlooktaskfolder-resource-type"></a>outlookTaskFolder 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含 Outlook 任务 （ [outlookTask](outlooktask.md)对象的集合） 的文件夹。 

在 Outlook 中，默认任务组中， `My Tasks`，包含默认任务文件夹， `Tasks`，用户的邮箱。 无法重命名或删除这些默认任务组和文件夹，但您可以创建其他任务组和任务文件夹。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 outlookTaskFolder](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |要获取的属性和指定 Outlook 任务文件夹的关系。|
|[创建 outlookTask](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| 在指定的任务文件夹中创建 Outlook 任务。|
|[List tasks](../api/outlooktaskfolder-list-tasks.md) |[outlookTask](outlooktask.md)集合| 在指定文件夹中获取所有 Outlook 任务。|
|[Update](../api/outlooktaskfolder-update.md) | [outlookTaskFolder](outlooktaskfolder.md)   |更新 Outlook 任务文件夹的可写属性。 |
|[Delete](../api/outlooktaskfolder-delete.md) | 无 |删除指定的 Outlook 任务文件夹。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |在新的或现有的 Outlook 任务文件夹中创建一个或多个单值扩展的属性。   |
|[使用单值扩展属性获取任务文件夹](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | 获取包含一个单值使用扩展属性的 Outlook 任务文件夹`$expand`或`$filter`。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | 在新的或现有的 Outlook 任务文件夹中创建一个或多个多值扩展的属性。  |
|[多值扩展属性获取任务文件夹](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | 获取包含多值扩展的属性，通过使用 Outlook 任务文件夹`$expand`。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|changeKey|String|任务文件夹的版本。|
|id|String|任务文件夹中，用户的邮箱中的唯一标识符。 只读。|
|isDefaultFolder|布尔值|如果文件夹为默认的任务文件夹，则为 true。|
|name|String|任务文件夹的名称。|
|parentGroupKey|Guid|任务文件夹的父组的唯一 GUID 标识符。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|multiValueLegacyExtendedProperty|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合|多值定义的任务文件夹的扩展属性的集合。 只读。 可为 NULL。|
|singleValueLegacyExtendedProperty|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection|定义的任务文件夹的单值扩展属性的集合。 只读。 可为 NULL。|
|tasks|[outlookTask](outlooktask.md)集合|此任务文件夹中的任务。 只读。 可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty",
    "tasks"
  ],
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
