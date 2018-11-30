---
title: assignedPlan 资源类型
description: 用户 实体和 组织 实体的 **AssignedPlans** 属性都是一个 **assignedPlan** 集合。
ms.openlocfilehash: 0df1540819b569b62607bf0e56c1c8f53d2749da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041762"
---
# <a name="assignedplan-resource-type"></a>assignedPlan 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[用户](user.md) 实体和 [组织](organization.md) 实体的 **AssignedPlans** 属性都是一个 **assignedPlan** 集合。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|分配计划的日期和时间；例如：2013-01-02T19:32:30Z。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|capabilityStatus|String|例如，“Enabled”。|
|服务|String|服务名称；例如，“Exchange”。|
|servicePlanId|Guid|用于标识服务计划的 GUID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
