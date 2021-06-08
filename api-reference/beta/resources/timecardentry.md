---
title: timeCardEntry 资源类型
description: 表示特定考勤卡条目。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d09b324b4d43765f05de789129021e2eb1f24789
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786382"
---
# <a name="timecardentry-resource-type"></a>timeCardEntry 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示特定 [timeCard](timecard.md) 条目。

## <a name="properties"></a>属性
|属性               |类型           |说明                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| clockInEvent       |[timeCardEvent](timecardevent.md)    | timeCard 的 **时钟事件**。|
| clockOutEvent                 |[timeCardEvent](timecardevent.md)  |timeCard 的 **时钟出事件**。 |
| breaks    |[timeCardBreak](timecardbreak.md) 集合    |与 **timeCard** 关联的中断列表。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEntry"
}-->
```json
{
   "clockInEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "clockOutEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "breaks":[
      {
         "breakId":"string",
         "notes":{
             "content": "string",
             "contentType": "text"
          },
         "start":{
            "dateTime":"String (timestamp)",
            "atApprovedLocation":true,
            "notes":{
                 "content": "string",
                 "contentType": "text"
            },
         },
         "end":null
      }
   ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timecardentry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
