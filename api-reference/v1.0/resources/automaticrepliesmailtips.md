---
title: automaticRepliesMailTips 资源类型
description: 有关在邮箱上设置的任何自动答复的邮件提示。
ms.localizationpriority: medium
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3e9904fe54d14fe707f4917934b81750aa9ec5fd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089863"
---
# <a name="automaticrepliesmailtips-resource-type"></a>automaticRepliesMailTips 资源类型

命名空间：microsoft.graph


[有关在](../resources/mailtips.md) 邮箱上设置的任何自动答复的邮件提示。

## <a name="properties"></a>属性
| 属性     | 类型   |描述|
|:-----|:-----|:-----|
| message | String | 自动答复邮件。 |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | 自动答复邮件使用的语言。 |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 自动答复设置为结束的日期和时间。 |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 自动答复设置为开始的日期和时间。 |

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

