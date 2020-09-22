---
title: regionalFormatOverrides 资源类型
description: 表示日历、日期和时间的区域格式替代的资源。
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 2ed130135571faeced90a638e9334a7e2a185a5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073505"
---
# <a name="regionalformatoverrides-resource-type"></a>regionalFormatOverrides 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示日历、日期和时间的格式重写的字符串的集合。 

## <a name="properties"></a>属性

|属性             |类型                 |说明                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|calendar             |String               |要使用的日历，例如公历。<br><br>默认情况下返回。|                   
|firstDayOfWeek       |String               |要使用的一周的第一天（例如，星期日）。<br><br>默认情况下返回。|
|shortDateFormat      |String               |要用于显示日期的短日期时间格式。<br><br>默认情况下返回。|
|longDateFormat       |String               |用于显示日期的长日期时间格式。<br><br>默认情况下返回。|
|shortTimeFormat      |String               |用于显示时间的短时间格式。<br><br>默认情况下返回。|
|longTimeFormat       |String               |用于显示时间的长时间格式。<br><br>默认情况下返回。|
|timeZone             |String               |要用于显示时间的时区。<br><br>默认情况下返回。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 定义。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "",
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


