---
title: plannerAppliedCategories 资源类型
description: '**AppliedCategoriesCollection**资源表示已应用于任务的类别（或标签）的集合。 它是 plannerTask 对象的一部分。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: bacf2ed499d420006173af8b3616a14b7c487904
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521816"
---
# <a name="plannerappliedcategories-resource-type"></a>plannerAppliedCategories 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**AppliedCategoriesCollection**资源表示已应用于任务的类别（或标签）的集合。 它是[plannerTask](plannertask.md)对象的一部分。
最多可以将6个类别应用于一个任务。 类别说明（如`category1` `category2`等）是 "[计划详细信息](plannerplandetails.md)" 对象的一部分。 这是开放类型。

## <a name="properties"></a>属性
可由客户端定义打开类型的属性。 但在这种情况下，客户端`category1`必须`category2`提供`category3`、 `category4`、 `category5` 、和/ `category6`或属性值作为属性，当`true`对该任务应用相应的类别时，这些属性的值为 boolean。 示例如下所示。 如果它们不适用，则通过将属性值设置为`false`布尔值来自动删除属性。 

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

示例： 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
