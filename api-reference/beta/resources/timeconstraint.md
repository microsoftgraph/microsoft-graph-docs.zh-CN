---
title: timeConstraint 资源类型
description: 根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。
ms.openlocfilehash: 092133d34e12fe5c06bfd8a76e8a33afb33892f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042698"
---
# <a name="timeconstraint-resource-type"></a>timeConstraint 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|activityDomain|字符串|（可选）活动性质。可取值为：`work`、`personal`、`unrestricted` 或 `unknown`。|
|timeslots|[timeSlot](timeslot.md) 集合|一组时间段。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->