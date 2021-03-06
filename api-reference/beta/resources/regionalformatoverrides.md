---
title: regionalFormatOverrides 资源类型
description: 表示日历、日期和时间的区域格式替代的资源。
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 2b4046ad8ec6b2d646d1dc2d93cbe7bed205cbad
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516064"
---
# <a name="regionalformatoverrides-resource-type"></a>regionalFormatOverrides 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示日历、日期和时间的格式替代的字符串集合。 

## <a name="properties"></a>属性

|属性             |类型                     |说明                                                    |
|---------------------|-------------------------|---------------------------------------------------------------|
|calendar             |String                   |要使用的日历，例如公历。<br><br>默认情况下返回。|                   
|firstDayOfWeek       |microsoft.graph.dayOfWeek|一周的第一天，例如，星期日。<br><br>默认情况下返回。|
|shortDateFormat      |String                   |用于显示日期的短日期时间格式。<br><br>默认情况下返回。|
|longDateFormat       |String                   |用于显示日期的长日期时间格式。<br><br>默认情况下返回。|
|shortTimeFormat      |String                   |用于显示时间的时间短格式。<br><br>默认情况下返回。|
|longTimeFormat       |String                   |用于显示时间的长期格式。<br><br>默认情况下返回。|
|timeZone             |String                   |用于显示时间的时间区。<br><br>默认情况下返回。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 定义。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.regionalFormatOverrides"
}-->

```json
{
    "calendar": "string",
    "firstDayOfWeek": "string",
    "shortDateFormat": "string",
    "longDateFormat": "string",
    "shortTimeFormat": "string",
    "longTimeFormat": "string",
    "timeZone": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalFormatOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


