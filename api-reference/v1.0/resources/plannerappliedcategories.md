---
title: plannerAppliedCategories 资源类型
description: '**AppliedCategoriesCollection**资源表示已应用于任务的类别 (或标签) 的集合。 它是 plannerTask 对象的一部分。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: fac4c69e9827e903d18f8665bc9b33e7c32705e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037624"
---
# <a name="plannerappliedcategories-resource-type"></a>plannerAppliedCategories 资源类型

命名空间：microsoft.graph


**AppliedCategoriesCollection**资源表示已应用于任务的类别 (或标签) 的集合。 它是 [plannerTask](plannertask.md) 对象的一部分。
最多可以将6个类别应用于一个任务。 类别说明（如 `category1` 等） `category2` 是 " [计划详细信息](plannerplandetails.md) " 对象的一部分。 这是开放类型。

## <a name="properties"></a>属性
可由客户端定义打开类型的属性。 但在这种情况下，客户端必须提供 `category1` 、 `category2` 、、 `category3` `category4` `category5` 和/或 `category6` 属性值作为属性，当对该 `true` 任务应用相应的类别时，这些属性的值为 boolean。 示例如下所示。 如果它们不适用，则通过将属性值设置为布尔值来自动删除属性 `false` 。 

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

