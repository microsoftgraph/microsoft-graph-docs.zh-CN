---
title: workingHours 资源类型
description: 表示特定时区用户一周的工作天数和小时数。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 775de66d328767e24a2bf7a47478cfcc2b482118e668ebf9c915eb069308f80a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182355"
---
# <a name="workinghours-resource-type"></a>workingHours 资源类型

命名空间：microsoft.graph

表示特定时区用户一周的工作天数和小时数。

在处理活动或资源规划应用场景中，访问用户的工作时间会有所帮助。 可以[获取](../api/user-get-mailboxsettings.md#example-3)用户的工作时间，并将其[设置](../api/user-update-mailboxsettings.md#example-2)为用户[邮箱设置](mailboxsettings.md)的一部分。 

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

