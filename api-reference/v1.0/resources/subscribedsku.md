---
title: subscribedSku 资源类型
description: 包含有关公司订阅的服务 SKU 的信息。
ms.localizationpriority: medium
author: SumitParikh
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ed4a509a0f222e0853848b99caf0bc4ddee31685
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333132"
---
# <a name="subscribedsku-resource-type"></a>subscribedSku 资源类型

命名空间：microsoft.graph

包含有关公司订阅的服务 SKU 的信息。

只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。

## <a name="methods"></a>Methods
| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 subscribedSku](../api/subscribedsku-get.md) | [subscribedSku](subscribedsku.md) |获取组织已获取的特定商业订阅。|
|[列出 subscribedsku](../api/subscribedsku-list.md) | [subscribedSku](subscribedsku.md) 集合 |获取组织已获取的商业版订阅的列表。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|appliesTo|String| 例如，“用户”或“公司”。 |
|capabilityStatus|String|  可取值为：`Enabled`、`Warning`、`Suspended`、`Deleted`、`LockedOut`。 capabilityStatus 表示`Enabled`**预付费Units** 属性至少启用了 1 `LockedOut` 个单位，并且客户已取消订阅。 |
|consumedUnits|Int32| 已分配的许可证数量。 |
|id|String| 订阅的 sku 对象的唯一标识符。 键，不可为 null。 |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| 有关预付许可证的数量和状态的信息。 |
|servicePlans|[servicePlanInfo](serviceplaninfo.md) collection| 有关 SKU 可用服务计划的信息。 不可为 null |
|skuId|Guid| 服务 SKU 的唯一标识符 (GUID)。 |
|skuPartNumber|String| SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。 若要获取组织已获取的商业订阅的列表，请参阅 [列出 subscribedSkus](../api/subscribedsku-list.md)。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "String",
  "capabilityStatus": "String",
  "consumedUnits": 1024,
  "id": "String (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

## <a name="see-also"></a>另请参阅

+ [许可的产品名称和服务计划标识符](/azure/active-directory/enterprise-users/licensing-service-plan-reference)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

