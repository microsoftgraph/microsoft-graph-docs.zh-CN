---
title: bookingWorkTimeSlot 资源类型
description: 定义工作的开始时间和结束时间。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 7b20514b52cbea033d3a4bccbca6def8f09ce46b
ms.sourcegitcommit: 94dc71a6d4fbdc46f2681a1add13416bc9b4a6e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2021
ms.locfileid: "60115286"
---
# <a name="bookingworktimeslot-resource-type"></a>bookingWorkTimeSlot 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
定义工作的开始时间和结束时间。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|end|TimeOfDay|一天中停止工作的时间。 例如，17：00：00.0000000。|
|start|TimeOfDay|一天中工作开始的时间。 例如，08：00：00.0000000。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkTimeSlot"
}-->

```json
{
  "end": "String (timestamp)",
  "start": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


