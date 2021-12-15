---
title: bookingSchedulingPolicy 资源类型
description: 代表一组策略，用于确定如何在 Microsoft Bookings 日历中创建约会。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 6df5bb71fdcd2710aa3970e398e5ec0def0eef89
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526517"
---
# <a name="bookingschedulingpolicy-resource-type"></a>bookingSchedulingPolicy 资源类型

命名空间：microsoft.graph

代表一组策略，用于确定如何在 Microsoft Bookings 日历中创建约会。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowStaffSelection|Boolean|如此 如果允许客户为预订选择特定人员。|
|maximumAdvance|期限|可以提前进行预订的最大天数。 它遵循 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式。|
|minimumLeadTime|期限|必须完成预定和取消的最小时间。 它遵循 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式。|
|sendConfirmationsToOwner|Boolean| 如果为 True，则创建或更改预订时通过电子邮件通知企业。 使用在 business 的 **bookingBusiness****实体的电子邮件** 属性中指定的电子邮件地址。 |
|timeSlotInterval|期限|每个时间段的持续时间，以 ISO [8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。|

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


