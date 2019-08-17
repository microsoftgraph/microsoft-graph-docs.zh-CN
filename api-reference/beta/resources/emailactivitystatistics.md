---
title: emailActivityStatistics 资源类型
description: 表示有关用户的电子邮件活动的其他信息
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ff75545b7f591a920ed4a1ffd65bff40cff8439b
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450725"
---
# <a name="emailactivitystatistics-resource-type"></a>emailActivityStatistics 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关用户在 Microsoft Outlook 的电子邮件活动中所用时间的数据。 这基于[activityStatistics](../resources/activitystatistics.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|activity|analyticsActivityType| 返回其统计信息的电子邮件活动。|
|duration|持续时间|在电子邮件上花费的总小时数。 值以 ISO 8601 格式表示, 持续时间。|
|endDate|Date|电子邮件活动结束的日期。 对于日历日期, 该值以 ISO 8601 格式表示。 例如, 属性值可以是 "2019-07-04", 它遵循 YYYY-MM-DD 格式。|
|id|String| 电子邮件活动的只读 ID。|
|startDate|日期|电子邮件活动的开始日期。 对于日历日期, 该值以 ISO 8601 格式表示。 例如, 属性值可以是 "2019-07-03", 它遵循 YYYY-MM-DD 格式。|
|timeZoneUsed|String|用户在 Outlook 日历中设置的时区用于计算。 例如, 属性值可以是 "太平洋标准时间"。|
|afterHours|持续时间|在工作时间之外的电子邮件上花费的总小时数, 基于用户的 Outlook 日历设置的工作时间。 值以 ISO 8601 格式表示, 持续时间。 |
|readEmail|持续时间|阅读电子邮件所用的总小时数。 值以 ISO 8601 格式表示, 持续时间。|
|sentEmail|持续时间|撰写和发送电子邮件所用的总小时数。 值以 ISO 8601 格式表示, 持续时间。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)",
  "readEmail": "String (ISO 8601 duration)",
  "sentEmail": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->