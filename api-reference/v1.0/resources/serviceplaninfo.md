---
title: servicePlanInfo 资源类型
description: 包含与订阅的 SKU 相关的服务计划有关的信息。**subscribedSku** 实体的 servicePlans 属性是一个 **servicePlanInfo** 集合。
ms.localizationpriority: medium
author: jpettere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 1f8da276ccbd0f22023550797f1563939e6e7e39
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126658"
---
# <a name="serviceplaninfo-resource-type"></a>servicePlanInfo 资源类型

命名空间：microsoft.graph

包含与订阅的 SKU 相关的服务计划有关的信息。**subscribedSku** 实体的 [servicePlans](subscribedsku.md) 属性是一个 **servicePlanInfo** 集合。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|servicePlanId|Guid|服务计划的唯一标识符。|
|servicePlanName|String|服务计划的名称。|
|provisioningStatus|String|服务计划的预配状态。 可能的值：<br/>"成功"- 服务已完全预配。<br/>"已禁用"- 服务已禁用。<br/>"PendingInput"- 服务尚未设置;等待服务确认。<br/>"PendingActivation"- 服务已设置，但需要管理员 (，例如，Intune_O365计划) <br/>"PendingProvisioning"- Microsoft 向产品 SKU 添加了新服务，但尚未在租户中激活。|
|appliesTo|String|可以为其分配服务计划的对象。 可能的值：<br/>"用户"- 可以将服务计划分配给单个用户。<br/>"公司"- 可以将服务计划分配给整个租户。|

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

