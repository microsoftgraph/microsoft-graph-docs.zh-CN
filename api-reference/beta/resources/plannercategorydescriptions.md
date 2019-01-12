---
title: plannerCategoryDescriptions 资源类型
description: '**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于计划详细信息对象。最多可定义 6 个类别。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4175692182d115e884642ef8f9956cc4db5dae2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930941"
---
# <a name="plannercategorydescriptions-resource-type"></a>plannerCategoryDescriptions 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于[计划详细信息](plannerplandetails.md)对象。最多可定义 6 个类别。 


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|category1|String|与类别 1 相关联的标签|
|category2|String|与类别 2 相关联的标签|
|category3|String|与类别 3 相关联的标签|
|category4|String|与类别 4 相关联的标签|
|category5|String|与类别 5 相关联的标签|
|category6|String|与类别 6 相关联的标签|

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
