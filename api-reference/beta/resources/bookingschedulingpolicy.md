---
title: bookingSchedulingPolicy 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 77b1cf812edd334197c268c92bb982954fb11b12
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974116"
---
# <a name="bookingschedulingpolicy-resource-type"></a>bookingSchedulingPolicy 资源类型

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示一组策略, 这些策略确定应如何在 Microsoft 预定日历中创建约会。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowStaffSelection|Boolean|如此如果允许客户选择预订的特定人员。|
|maximumAdvance|持续时间|可以提前进行预订的最大天数。 它遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。|
|minimumLeadTime|持续时间|在必须进行预订和取消的前的最小时间量。 它遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。|
|sendConfirmationsToOwner|Boolean| 真要在创建或更改预订时通过电子邮件通知商业。 使用在企业的**bookingBusiness**实体的**email**属性中指定的电子邮件地址。 |
|timeSlotInterval|持续时间|每个时间段的持续时间, 以[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。|

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
