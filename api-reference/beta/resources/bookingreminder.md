---
title: bookingReminder 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 039f01375b2483f1bda1a63e999556d194fae048
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457427"
---
# <a name="bookingreminder-resource-type"></a>bookingReminder 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示何时以及何时发送电子邮件提醒。


## <a name="properties"></a>属性
| 属性     | 类型   |描述|
|:---------------|:--------|:----------|
|message|String|提醒中的邮件。|
|一定|持续时间|约会开始前的时间量应发送提醒。 它以[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。|
|recipients|String| Shouold 收到提醒的人员。 可取值为：`allAttendees`、`staff`、`customer`。|

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
  "recipients": "String"
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
