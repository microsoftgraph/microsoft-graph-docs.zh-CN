---
title: privilegedRoleSettings 资源类型
description: 代表特权角色的设置。
ms.openlocfilehash: 14b4919d653de80c97f06aff507c011162c3c0e4
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2018
ms.locfileid: "27049557"
---
# <a name="privilegedrolesettings-resource-type"></a>privilegedRoleSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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

## <a name="relationships"></a>Relationships
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->