---
title: subscribedSku 资源类型
description: " 创建、 更新和删除不受支持。 不支持查询筛选器表达式。 继承自 directoryObject。"
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01dbbf8727ab361b3763e2343e7cc72a3676848b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960152"
---
# <a name="subscribedsku-resource-type"></a>subscribedSku 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。


## <a name="methods"></a>方法
| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 subscribedSku](../api/subscribedsku-get.md) | [subscribedSku](subscribedsku.md) |读取 subscribedSku 对象的属性和关系。|
|[列表 subscribedsku](../api/subscribedsku-list.md) | [subscribedSku](subscribedsku.md) 集合 |检索组织已获取的商业订阅列表。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|appliesTo|String| 例如，“用户”或“公司”。 |
|capabilityStatus|String| 例如，“Enabled”。 |
|consumedUnits|Int32| 已分配的许可证数量。 |
|id|String| 订阅的 sku 对象的唯一标识符。密钥，不可为 NULL。 |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| 有关预付许可证的数量和状态的信息。 |
|servicePlans|[servicePlanInfo](serviceplaninfo.md) collection| 有关 SKU 可用服务计划的信息。不可为 null |
|skuId|Guid| 服务 SKU 的唯一标识符 (GUID)。 |
|skuPartNumber|字符串| SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。 |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
