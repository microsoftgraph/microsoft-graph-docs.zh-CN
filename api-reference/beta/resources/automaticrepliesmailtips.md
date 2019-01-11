---
title: automaticRepliesMailTips 资源类型
description: 有关对邮箱设置任何自动答复邮件提示。
localization_priority: Normal
ms.openlocfilehash: 80ecaaa9fced0bcb00494b0414a86f0a11fd8996
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833227"
---
# <a name="automaticrepliesmailtips-resource-type"></a>automaticRepliesMailTips 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

有关对邮箱设置任何自动答复[邮件提示](../resources/mailtips.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:-----|:-----|:-----|
| message | 字符串 | 自动答复邮件。 |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | 一种语言中的自动答复邮件。 |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 日期和时间的自动答复设置结束。 |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 日期和时间的自动答复设置开始。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
