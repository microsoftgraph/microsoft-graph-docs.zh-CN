---
title: workingHours 资源类型
description: 表示特定时区用户一周的工作天数和小时数。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c3449e64f94a3e90bae443a23e7b941116df0291
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033325"
---
# <a name="workinghours-resource-type"></a>workingHours 资源类型

表示特定时区用户一周的工作天数和小时数。

在处理活动或资源规划应用场景中，访问用户的工作时间会有所帮助。 可以[获取](../api/user-get-mailboxsettings.md#request-3)用户的工作时间，并将其[设置](../api/user-update-mailboxsettings.md#request-2)为用户[邮箱设置](mailboxsettings.md)的一部分。 

可以选择以不同于在 Outlook 客户端设置时区的方式，为你的工作时间设置时区。 在某些情况下这很有用，比如当你在一个与平常工作时区不同的地方旅行时。 可以将 Outlook 客户端设置  
为目标时区，以便在你访问时 Outlook 时间值显示为本地时间。
当其他人在你通常的工作地点申请与你进行工作会议时，他们仍然可以在相应的时区遵守你的工作时间。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| daysOfWeek | dayOfWeek 集合 | 用户一周工作的天数。 |
| startTime | Edm.TimeOfDay | 一天中用户开始工作的时间。 |
| endTime | Edm.TimeOfDay | 一天中用户停止工作的时间。 |
| timeZone | [timeZoneBase](timezonebase.md) | 工作时间应用的时区。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "String (timeofday)",
  "endTime": "String (timeofday)",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/workinghours.md/microsoft.graph.workingHours/daysOfWeek:
      Inconsistent types between parameter (String) and table (Object)"
  ],
  "tocPath": ""
}-->
