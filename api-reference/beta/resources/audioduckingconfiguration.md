---
title: audioDuckingConfiguration 资源类型
description: 参数放掉的其他源 （逐步注销其他源。）
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4132946573342976bb1f20c593454a8e18030d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916871"
---
# <a name="audioduckingconfiguration-resource-type"></a>audioDuckingConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

参数放掉的其他源 （逐步注销其他源。）

## <a name="properties"></a>属性

| 属性      | 类型     | Description                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| lowerLevel    | Int64    | 源中时源正在 ducked %的卷。             |
| rampActive    | Int64    | 时间 （以毫秒计） 计的 ducked 源以"淡出"。 |
| rampInactive  | Int64    | 时间 （以毫秒计） 计的 ducked 源"淡出"。  |
| upperLevel    | Int64    | 源中时源不正在 ducked %的卷。         |

> **注意：** 提升持续时间不能超过 5000 毫秒。

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
<!-- {
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
