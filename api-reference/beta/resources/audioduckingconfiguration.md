---
title: audioDuckingConfiguration 资源类型
description: 其他源的 ducking 参数 (逐步淘汰 in 和其他来源。)
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cfff0ca240a13c9c4396d605def05a52e1916778
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013218"
---
# <a name="audioduckingconfiguration-resource-type"></a>audioDuckingConfiguration 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

其他源的 ducking 参数 (逐步淘汰 in 和其他来源。)

## <a name="properties"></a>属性

| 属性      | 类型     | 说明                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| lowerLevel    | Int64    | 源正在 ducked 时, 源的数量 (以百分比为单位)。             |
| rampActive    | Int64    | Ducked 源到 "淡出" 所需的时间量 (以毫秒为单位)。 |
| rampInactive  | Int64    | Ducked 源到 "淡入" 所需的时间 (以毫秒为单位)。  |
| upperLevel    | Int64    | 源未 ducked 时的源数量 (以百分比为单位)。         |

> **注意:** 斜向持续时间不能超过5000毫秒。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
