---
title: privilegedRoleSettings 资源类型
description: 表示特权角色的设置。
localization_priority: Normal
ms.openlocfilehash: 7d4c14065defc63190d1d25b435c734b9f219e36
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563246"
---
# <a name="privilegedrolesettings-resource-type"></a>privilegedRoleSettings 资源类型

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
|isMfaOnElevationConfigurable|布尔|如果 mfaOnElevation 是可配置的,**则为 true** 。 **假**如果 mfaOnElevation 不可配置。|
|lastGlobalAdmin|布尔|仅供内部使用。|
|maxElavationDuration|duration|已激活角色的最大持续时间。|
|mfaOnElevation|布尔|如果需要 MFA 以激活角色,**则为 true** 。 **假**如果无需进行 MFA 即可激活角色。|
|minElevationDuration|duration|已激活角色的最短持续时间。|
|notificationToUserOnElevation|布尔|如果激活角色时向最终用户发送通知,**则为 true** 。 **假**如果在角色激活时不发送通知。|
|ticketingInfoOnElevation|布尔|如果激活角色时需要票证信息,**则为 true** 。 **假**如果激活角色时不需要票证信息。|
|approvalOnElevation|布尔|如果激活角色时需要进行审批,**则为 true** 。 **假**如果激活该角色时不需要审批。|
|approverIds|数组|审批 id 的列表 (如果激活需要审批)。|

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
