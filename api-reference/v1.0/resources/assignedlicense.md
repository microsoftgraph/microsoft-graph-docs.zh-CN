---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。 User 实体的 **assignedLicenses** 属性是 **assignedLicense**的集合。
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a4193e09b756437d693e484a0680c27c4e8b6013
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003281"
---
# <a name="assignedlicense-resource-type"></a>assignedLicense 资源类型

命名空间：microsoft.graph

表示分配给用户的许可证。 [User](user.md)实体的**AssignedLicenses**属性是**assignedLicense**的集合。

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

