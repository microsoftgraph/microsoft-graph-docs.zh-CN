---
title: servicePlanInfo 资源类型
description: 包含与订阅的 SKU 相关的服务计划有关的信息。subscribedSku 实体的 **servicePlans** 属性是一个 **servicePlanInfo** 集合。
localization_priority: Normal
ms.openlocfilehash: 837170881c7c093d26c5b59662e20e87b399a029
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845449"
---
# <a name="serviceplaninfo-resource-type"></a>servicePlanInfo 资源类型

包含与订阅的 SKU 相关的服务计划有关的信息。[subscribedSku](subscribedsku.md) 实体的 **servicePlans** 属性是一个 **servicePlanInfo** 集合。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|servicePlanId|Guid|服务计划的唯一标识符。|
|servicePlanName|String|服务计划的名称。|
|provisioningStatus|字符串|服务计划的预配状态。可能的值：<br/>“Success” - 服务已完全预配。<br/>“Disabled” - 服务已禁用。<br/>“PendingInput” - 服务尚未预配；等待服务确认。<br/>“PendingActivation” - 服务已预配，但需要由管理员显式激活（例如，Intune_O365 服务计划）<br/>“PendingProvisioning” - Microsoft 已将新服务添加到产品 SKU，但它尚未在租户中激活。|
|appliesTo|字符串|可以向其分配服务计划的对象。可能的值：<br/>“User” - 服务计划可分配给各个用户。<br/>“Company” - 服务计划可分配给整个租户。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
