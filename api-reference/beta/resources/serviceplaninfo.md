---
title: servicePlanInfo 资源类型
description: 包含与订阅的 SKU 相关联的服务计划的相关信息。 SubscribedSku 实体的 **servicePlans** 属性是 **servicePlanInfo**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: ab76cced936ebaa9f69a7fe7d4a2c2c4909475d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019486"
---
# <a name="serviceplaninfo-resource-type"></a>servicePlanInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与订阅的 SKU 相关联的服务计划的相关信息。 [SubscribedSku](subscribedsku.md)实体的**ServicePlans**属性是**servicePlanInfo**的集合。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|servicePlanId|Guid|服务计划的唯一标识符。|
|servicePlanName|String|服务计划的名称。|
|provisioningStatus|String|服务计划的预配状态。 可能的值：<br/>"成功"-服务已完全预配。<br/>"已禁用"-服务已禁用。<br/>"PendingInput"-服务尚未预配;等待服务确认。<br/>"PendingActivation"-服务已预配，但需要管理员进行显式激活 (例如，Intune_O365 Service plan) 。<br/>"PendingProvisioning"-Microsoft 已向产品 SKU 添加了新服务，但尚未在租户中激活。|
|appliesTo|String|可将服务计划分配到的对象。 可能的值：<br/>"User"-服务计划可分配给单个用户。<br/>"Company"-服务计划可分配给整个租户。|

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
<!--
{
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


