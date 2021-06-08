---
title: timeCardEvent 资源类型
description: 表示特定时间卡事件。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a8be7d000b3d55368f7378e9b993b5015b7ef632
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786367"
---
# <a name="timecardevent-resource-type"></a>timeCardEvent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示特定 [timeCard](timecard.md) 事件。

## <a name="properties"></a>属性
|属性               |类型           |说明                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| dateTime                  |`Edm.dateTimeOffset`  |记录条目的时间。 |
| atApprovedLocation |`Edm.boolean `  |指示条目是否记录在已批准的位置。 |
| notes                 |[itemBody](itembody.md)  | 有关 **timeCardEvent 的注释**。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEvent"
}-->
```json
{
   "atApprovedLocation":true,
   "notes":{ "@odata.type":"microsoft.graph.itemBody" }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
