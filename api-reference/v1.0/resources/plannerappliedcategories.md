---
title: plannerAppliedCategories 资源类型
description: '**AppliedCategoriesCollection** 资源表示已 (任务) 或标签的类别集合。 它是 plannerTask 对象的一部分。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7095c2f2069b89009c9f8cdbe5908812dd03620f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044396"
---
# <a name="plannerappliedcategories-resource-type"></a>plannerAppliedCategories 资源类型

命名空间：microsoft.graph


**AppliedCategoriesCollection** 资源表示已 (任务) 或标签的类别集合。 它是 [plannerTask 对象的一](plannertask.md) 部分。
最多只能有 6 个类别应用于任务。 类别说明（如 等） `category1` 是 `category2` 计划详细信息 [对象的一](plannerplandetails.md) 部分。 这是开放类型。

## <a name="properties"></a>属性
开放类型的属性可通过客户端定义。 但在这种情况下，客户端必须提供 、 和/或 属性，当相应类别应用于任务时，其值为 `category1` `category2` `category3` `category4` `category5` `category6` `true` 布尔值。 示例如下所示。 如果这些属性不适用，则会自动删除属性的值设置为 `false` 布尔值。 

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

