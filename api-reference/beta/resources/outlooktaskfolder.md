---
title: outlookTaskFolder 资源类型
description: '包含 Outlook 任务的文件夹 () 的 outlookTask 对象的集合。 '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c9f9958750cca1aaa40ba9394832e5974bed8cc3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998360"
---
# <a name="outlooktaskfolder-resource-type-deprecated"></a>outlookTaskFolder 资源类型 (弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


包含 Outlook 任务的文件夹 () 的 [outlookTask](outlooktask.md) 对象的集合。 

在 Outlook 中，默认任务组， `My Tasks` 包含用户邮箱的默认任务文件夹 `Tasks` 。 您不能重命名或删除这些默认任务组和文件夹，但可以创建其他任务组和任务文件夹。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 outlookTaskFolder](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |获取指定的 Outlook 任务文件夹的属性和关系。|
|[创建 outlookTask](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| 在指定的任务文件夹中创建一个 Outlook 任务。|
|[列出任务](../api/outlooktaskfolder-list-tasks.md) |[outlookTask](outlooktask.md) 集合| 获取指定文件夹中的所有 Outlook 任务。|
|[更新](../api/outlooktaskfolder-update.md) | [outlookTaskFolder](outlooktaskfolder.md)   |更新 Outlook 任务文件夹的可写属性。 |
|[删除](../api/outlooktaskfolder-delete.md) | 无 |删除指定的 Outlook 任务文件夹。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |在新的或现有的 Outlook 任务文件夹中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的任务文件夹](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | 通过使用或获取包含单值扩展属性的 Outlook 任务文件夹 `$expand` `$filter` 。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | 在新的或现有的 Outlook 任务文件夹中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的任务文件夹](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | 使用获取包含多值扩展属性的 Outlook 任务文件夹 `$expand` 。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|changeKey|String|任务文件夹的版本。|
|id|String|任务文件夹的标识符，在用户的邮箱中是唯一的。 只读。|
|isDefaultFolder|Boolean|如此如果该文件夹是默认的任务文件夹。|
|name|String|任务文件夹的名称。|
|parentGroupKey|Guid|任务文件夹的父组的唯一 GUID 标识符。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合|为任务文件夹定义的多值扩展属性的集合。 只读。 可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合|为任务文件夹定义的单值扩展属性的集合。 只读。 可为 Null。|
|任务|[outlookTask](outlooktask.md) 集合|此任务文件夹中的任务。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
  "suppressions": []
}
-->


