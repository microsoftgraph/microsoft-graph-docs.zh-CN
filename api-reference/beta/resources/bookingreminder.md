---
title: bookingReminder 资源类型
description: 表示电子邮件提醒的发送时间及发送者。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 51dde51c25064edb0c6548676bb7921b7705dcf2
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524677"
---
# <a name="bookingreminder-resource-type"></a>bookingReminder 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示电子邮件提醒的发送时间及发送者。


## <a name="properties"></a>属性
| 属性     | 类型   |描述|
|:---------------|:--------|:----------|
|message|String|提醒中的消息。|
|offset|期限|约会开始前应发送提醒的时间量。 它以 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。|
|recipients|bookingReminderRecipients| 应接收提醒的人员。 可能的值是 `allAttendees` ：、 `staff` 和 `customer` `unknownFutureValue` 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingReminder"
}-->

```json
{
  "message": "String",
  "offset": "String (timestamp)",
  "recipients": {"@odata.type": "microsoft.graph.bookingReminderRecipients"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


