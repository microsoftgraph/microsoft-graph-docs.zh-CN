---
title: licenseDetails 资源类型
description: 包含有关分配给用户的许可证的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 12e0dcb86288eb27859b87a1029e89676a5d511b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966955"
---
# <a name="licensedetails-resource-type"></a>licenseDetails 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关分配给用户的许可证的信息。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List licenseDetails](../api/user-list-licensedetails.md) | licenseDetails 集合 |检索用户的 licenseDetails 对象列表。|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 许可证详细信息对象的唯一标识符。 只读、键、不可为 null |
|servicePlans|[servicePlanInfo](serviceplaninfo.md) collection| 有关使用许可证分配的服务计划的信息。 只读, 不可为 null |
|skuId|Guid| 服务 SKU 的唯一标识符 (GUID)。 等于相关[SubscribedSku](subscribedsku.md)对象的 skuId 属性。 只读 |
|skuPartNumber|String| 唯一 SKU 显示名称。 等于相关[SubscribedSku](subscribedsku.md)对象上的 skuPartNumber;例如: "AAD_Premium"。 只读 |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
