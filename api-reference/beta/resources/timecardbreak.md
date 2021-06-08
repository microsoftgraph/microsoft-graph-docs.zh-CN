---
title: timeCardBreak 资源类型
description: 表示特定时间卡中断。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 509667ec1fad41f956ee5ee6d6a4371b8d17fc2e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786366"
---
# <a name="timecardbreak-resource-type"></a>timeCardBreak 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示特定 [timeCard](timecard.md) 中断。

## <a name="properties"></a>属性
|属性               |类型           |说明                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| breakId                   |`Edm.string`  |**timeCardBreak** 的 ID。|
| start                 |[timeCardEvent](timecardevent.md)    | **timeCardBreak 的开始事件**。|
| end                   |[timeCardEvent](timecardevent.md)    | **timeCardBreak 的开始事件**。|
| notes                 |[itemBody](itembody.md)  | 有关 **timeCardBreak 的注释**。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardBreak"
}-->
```json
{
    "breakId":"string",
    "notes":{
        "content": "string",
        "contentType": "string"
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
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardBreak resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
