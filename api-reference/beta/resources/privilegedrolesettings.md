---
title: privilegedRoleSettings 资源类型
description: 表示特权角色的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a1f20455ffcc818aa1b1edf784d6990d68b7556b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962565"
---
# <a name="privilegedrolesettings-resource-type"></a>privilegedRoleSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示特权角色的设置。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |读取 privilegedRoleSettings 对象的属性和关系。|
|[更新 privilegedRoleSettings](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |更新 privilegedRoleSettings 对象。|
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|elevationDuration|duration|角色激活的持续时间。|
|id|string| 角色设置的唯一标识符。 只读。|
|isMfaOnElevationConfigurable|boolean|`true` 如果 **mfaOnElevation** 可配置。 `false` 如果 **mfaOnElevation** 不可配置。|
|lastGlobalAdmin|boolean|仅内部使用。|
|maxEationDuration|duration|已激活角色的最长持续时间。|
|mfaOnElevation|boolean|`true` 如果激活角色需要 MFA。 `false` 如果不需要 MFA 即可激活角色。|
|minElevationDuration|duration|已激活角色的最短持续时间。|
|notificationToUserOnElevation|boolean|`true` 如果激活角色时向最终用户发送通知。 `false` 如果角色激活时不发送通知。|
|ticketingInfoOnElevation|boolean|`true` 如果激活角色时需要票证信息。 `false` 如果激活角色时不需要票证信息。|
|approvalOnElevation|boolean|`true` 如果激活角色时需要审批。 `false` 如果激活角色时不需要审批。|
|approverIds| string 集合 |审批 ID 列表（如果需要审批才能激活）。|

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


