---
title: plannerCategoryDescriptions 资源类型
description: '**plannerCategoryDescriptions** 资源表示为计划定义的类别的描述性标签。 它属于计划详细信息对象。 可以定义最多 6 个类别。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 5dcb6a9b2825b2a246f1bef9b55c453c6c53c1d8c6e56a45474bfa804d8caa15
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54154915"
---
# <a name="plannercategorydescriptions-resource-type"></a>plannerCategoryDescriptions 资源类型

命名空间：microsoft.graph

**plannerCategoryDescriptions** 资源表示为计划定义的类别的描述性标签。 它属于计划 [详细信息](plannerplandetails.md) 对象。 可以定义最多 6 个类别。 


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|category1|String|与类别 1 关联的标签|
|category2|String|与类别 2 关联的标签|
|category3|String|与类别 3 关联的标签|
|category4|String|与类别 4 关联的标签|
|category5|String|与类别 5 关联的标签|
|category6|String|与类别 6 关联的标签|

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

