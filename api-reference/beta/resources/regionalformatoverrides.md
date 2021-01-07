---
title: regionalFormatOverrides 资源类型
description: 表示日历、日期和时间的区域格式替代的资源。
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 437b67f6a99017bb20096dbd20451b7662145cbd
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777594"
---
# <a name="regionalformatoverrides-resource-type"></a>regionalFormatOverrides 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示日历、 日期和时间的格式替代的字符串的集合。 

## <a name="properties"></a>属性

|属性             |类型                 |说明                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|calendar             |String               |要使用的日历，例如公历。<br><br>默认情况下返回。|                   
|firstDayOfWeek       |String               |一周的第一天，例如星期日。<br><br>默认情况下返回。|
|shortDateFormat      |String               |用于显示日期的短日期时间格式。<br><br>默认情况下返回。|
|longDateFormat       |String               |用于显示日期的长日期时间格式。<br><br>默认情况下返回。|
|shortTimeFormat      |String               |用于显示时间的时间的短时间格式。<br><br>默认情况下返回。|
|longTimeFormat       |String               |用于显示时间的长期格式。<br><br>默认情况下返回。|
|timeZone             |String               |用于显示时间的时间区。<br><br>默认情况下返回。|

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


