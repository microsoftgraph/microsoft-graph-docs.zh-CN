---
title: privilegedRoleSettings 资源类型
description: 表示特权角色的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 7a082804309799c946f05f21d37d92b2eded7d13
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070504"
---
# <a name="privilegedrolesettings-resource-type"></a>privilegedRoleSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示特权角色的设置。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |读取 privilegedRoleSettings 对象的属性和关系。|
|[更新 privilegedRoleSettings](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |更新 privilegedRoleSettings 对象。|
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|elevationDuration|duration|激活角色的持续时间。|
|id|string| 角色设置的唯一标识符。 只读。|
|isMfaOnElevationConfigurable|boolean|如果 mfaOnElevation 是可配置的，**则为 true** 。 **假** 如果 mfaOnElevation 不可配置。|
|lastGlobalAdmin|boolean|仅供内部使用。|
|maxElavationDuration|duration|已激活角色的最大持续时间。|
|mfaOnElevation|boolean|如果需要 MFA 以激活角色，**则为 true** 。 **假** 如果无需进行 MFA 即可激活角色。|
|minElevationDuration|duration|已激活角色的最短持续时间。|
|notificationToUserOnElevation|boolean|如果激活角色时向最终用户发送通知，**则为 true** 。 **假** 如果在角色激活时不发送通知。|
|ticketingInfoOnElevation|boolean|如果激活角色时需要票证信息，**则为 true** 。 **假** 如果激活角色时不需要票证信息。|
|approvalOnElevation|boolean|如果激活角色时需要进行审批，**则为 true** 。 **假** 如果激活该角色时不需要审批。|
|approverIds| string 集合 |审批 id 的列表（如果激活需要审批）。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


