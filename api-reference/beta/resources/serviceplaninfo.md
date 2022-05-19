---
title: servicePlanInfo 资源类型
description: 包含与订阅的 SKU 相关的服务计划有关的信息。**subscribedSku** 实体的 servicePlans 属性是一个 **servicePlanInfo** 集合。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: jconley76
ms.openlocfilehash: 7cf978941ca634cf64168b388eb9a01f4da2b068
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549496"
---
# <a name="serviceplaninfo-resource-type"></a>servicePlanInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与订阅的 SKU 相关的服务计划有关的信息。**subscribedSku** 实体的 [servicePlans](subscribedsku.md) 属性是一个 **servicePlanInfo** 集合。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|servicePlanId|Guid|服务计划的唯一标识符。|
|servicePlanName|String|服务计划的名称。|
|provisioningStatus|String|服务计划的预配状态。 可能的值有：<br/>`Success` - 服务已完全预配。<br/>`Disabled` - 服务已禁用。<br/>`ErrorStatus` - 尚未预配服务计划，并且处于错误状态。<br/>`PendingInput` - 尚未预配服务;等待服务确认。<br/>`PendingActivation` - 服务已预配，但需要管理员 (显式激活，例如，Intune_O365服务计划) <br/>`PendingProvisioning` - Microsoft 已将新服务添加到产品 SKU，但尚未在租户中激活该服务。|
|appliesTo|String|服务计划可以分配给的对象。 可能的值有：<br/>`User` - 服务计划可以分配给单个用户。<br/>`Company` - 服务计划可以分配给整个租户。|

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
  "appliesTo": "String",
  "provisioningStatus": "String",
  "servicePlanId": "Guid",
  "servicePlanName": "String"
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


