---
title: bookingSchedulingPolicy 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 039d76b00787c9bf2e4f0bee4eb927a7628a9e76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914635"
---
# <a name="bookingschedulingpolicy-resource-type"></a>bookingSchedulingPolicy 资源类型

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。
 
代表确定应如何在 Microsoft 预订日历中创建约会的策略的组。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|allowStaffSelection|布尔|True 如果以使客户能够选择特定预定的人员。|
|maximumAdvance|Duration|最大天数提前所能进行预订。 遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。|
|minimumLeadTime|Duration|最小在其前面预订和取消通知必须进行的时间量。 遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。|
|sendConfirmationsToOwner|布尔| 预定会创建或更改时通知通过电子邮件的业务，则为 true。 使用业务**bookingBusiness**实体的**email**属性中指定的电子邮件地址。 |
|timeSlotInterval|Duration|[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式中每个时间段的持续时间。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
