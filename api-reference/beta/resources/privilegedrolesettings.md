---
title: privilegedRoleSettings 资源类型
description: 表示特权角色的设置。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 6c91003b7aa0455c6dd56b374fb45c3664111be3
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397477"
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
|elevationDuration|duration|激活角色时的持续时间。|
|id|string| 角色设置的唯一标识符。 只读。|
|isMfaOnElevationConfigurable|boolean|`true` 如果 **mfaOnElevation** 是可配置的， `false` 如果 **无法配置 mfaOnElevation，则为 mfaOnElevation** 。|
|lastGlobalAdmin|boolean|仅内部使用。|
|maxElavationDuration|duration|激活角色的最大持续时间。|
|mfaOnElevation|boolean|`true` 如果需要 MFA 来激活角色。 `false` 如果不需要 MFA 来激活角色。|
|minElevationDuration|duration|激活角色的最短持续时间。|
|notificationToUserOnElevation|boolean|`true` 如果在激活角色时向最终用户发送通知。 `false` 如果激活角色时不发送通知。|
|ticketingInfoOnElevation|boolean|`true` 如果激活角色时需要票证信息， `false` 如果激活角色时不需要票证信息。|
|approvalOnElevation|boolean|`true` if the approval is required when activate the role. `false` 如果激活角色时不需要审批。|
|approverIds| 字符串集合 |如果激活需要审批，则为审批 ID 列表。|

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


