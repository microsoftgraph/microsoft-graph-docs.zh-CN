---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。**用户** 实体的 AssignedLicenses 属性是一个 **assignedLicense** 集合。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jconley76
ms.openlocfilehash: 0b1dc256016576f5a7759923c051a546e95a336a
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549594"
---
# <a name="assignedlicense-resource-type"></a>assignedLicense 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示分配给用户的许可证。**用户** 实体的 [AssignedLicenses](user.md) 属性是一个 **assignedLicense** 集合。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
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
  "disabledPlans": ["Guid"],
  "skuId": "Guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


