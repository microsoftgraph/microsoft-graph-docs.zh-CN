---
title: plannerCategoryDescriptions 资源类型
description: '**plannerCategoryDescriptions**资源表示已为计划定义的类别的描述性标签。 它属于 "计划详细信息" 对象。 最多可以定义6个类别。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a410f748c43d50872936d4bcc106ffeb224d76cf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344555"
---
# <a name="plannercategorydescriptions-resource-type"></a>plannerCategoryDescriptions 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerCategoryDescriptions**资源表示已为计划定义的类别的描述性标签。 它属于 "[计划详细信息](plannerplandetails.md)" 对象。 最多可以定义6个类别。 


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
<!--
{
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
