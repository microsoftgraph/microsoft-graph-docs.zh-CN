---
title: plannerCategoryDescriptions 资源类型
description: '**PlannerCategoryDescriptions**资源表示已为计划定义的类别的描述性标签。 它属于 "计划详细信息" 对象。 最多可以定义6个类别。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d0ef4c4f91c4b2f8017a7b7555785c9dd10d082a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447134"
---
# <a name="plannercategorydescriptions-resource-type"></a>plannerCategoryDescriptions 资源类型

命名空间： microsoft. graph

**PlannerCategoryDescriptions**资源表示已为计划定义的类别的描述性标签。 它属于 "[计划详细信息](plannerplandetails.md)" 对象。 最多可以定义6个类别。 


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|category1|String|与类别1关联的标签|
|category2|String|与类别2关联的标签|
|category3|String|与类别3相关联的标签|
|category4|String|与类别4关联的标签|
|category5|String|与类别5相关联的标签|
|category6|String|与类别6关联的标签|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
