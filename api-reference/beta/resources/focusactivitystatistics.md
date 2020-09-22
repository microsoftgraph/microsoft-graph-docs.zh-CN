---
title: focusActivityStatistics 资源类型
description: 表示有关用户的单个焦点工作的信息
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3da2dc2719f24bfd986d5a3df550b4635b734131
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052878"
---
# <a name="focusactivitystatistics-resource-type"></a>focusActivityStatistics 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关用户可用于焦点工作的时间的数据。 这基于 [activityStatistics](../resources/activitystatistics.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|activity|analyticsActivityType| 为其返回统计信息的焦点活动。|
|duration|持续时间|总的工作时间总和（相当于至少两个连续的小时）在用户的 Microsoft Outlook 日历中，在用户设置的工作时间内没有与其他人召开会议。 值以 ISO 8601 格式表示，持续时间。|
|endDate|日期|焦点活动结束的日期。 对于日历日期，该值以 ISO 8601 格式表示。 例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。|
|id|String| 焦点活动的只读 ID。|
|startDate|日期|焦点活动的开始日期。 对于日历日期，该值以 ISO 8601 格式表示。 例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。|
|timeZoneUsed|String|用户在 Outlook 日历中设置的时区用于计算。 例如，属性值可以是 "太平洋标准时间"。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.focusActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String"
  }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "focusActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

