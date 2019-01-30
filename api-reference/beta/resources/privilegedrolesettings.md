---
title: privilegedRoleSettings 资源类型
description: 代表特权角色的设置。
localization_priority: Normal
ms.openlocfilehash: 7d4c14065defc63190d1d25b435c734b9f219e36
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642777"
---
# <a name="privilegedrolesettings-resource-type"></a>privilegedRoleSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表特权角色的设置。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |读取属性和 privilegedRoleSettings 对象的关系。|
|[更新 privilegedRoleSettings](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |更新 privilegedRoleSettings 对象。|
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|elevationDuration|duration|当激活角色持续时间。|
|id|string| 角色设置唯一标识符。 只读。|
|isMfaOnElevationConfigurable|boolean|**true**如果 mfaOnElevation 可配置。 **false**如果 mfaOnElevation 不可配置。|
|lastGlobalAdmin|boolean|仅供内部。|
|maxElavationDuration|duration|激活角色的最大持续时间。|
|mfaOnElevation|boolean|如果为**true** MFA 需要激活角色。 **false**如果 MFA 不需要激活角色。|
|minElevationDuration|duration|最少持续时间激活角色。|
|notificationToUserOnElevation|boolean|**true**如果角色激活时向最终用户发送通知。 **false**如果角色被激活时不发送通知。|
|ticketingInfoOnElevation|boolean|如果为**true**时，票证信息是必需激活角色。 **false**如果票证信息不需要激活角色。|
|approvalOnElevation|boolean|**true**如果情况下审批，需要激活角色。 **false**如果审批不需要激活角色。|
|approverIds|array|审批 id，如果需要激活审核的列表。|

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
  "approverIds": []
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
