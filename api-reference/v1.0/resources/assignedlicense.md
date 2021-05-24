---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。**用户** 实体的 AssignedLicenses 属性是一个 **assignedLicense** 集合。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c5aceba073cf7962b7b1caeb9a25a1936d5d4248
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546957"
---
# <a name="assignedlicense-resource-type"></a>assignedLicense 资源类型

命名空间：microsoft.graph

表示分配给用户的许可证。**用户** 实体的 [AssignedLicenses](user.md) 属性是一个 **assignedLicense** 集合。

## <a name="properties"></a>属性
| 属性     | 类型   |描述|
|:---------------|:--------|:----------|
|disabledPlans|Guid 集合|已禁用的计划的唯一标识符的集合。|
|skuId|Guid|此 SKU 的唯一标识符。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

