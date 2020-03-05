---
title: callMediaState 资源类型
description: 表示呼叫的媒体状态。
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: c9c55908f62214c386aacee34be76bb11fc318b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507808"
---
# <a name="callmediastate-resource-type"></a>callMediaState 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[呼叫](call.md)的媒体状态。

## <a name="properties"></a>属性

| 属性            | 类型    | 说明                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| audio           | String  | 音频媒体状态。 可取值为：`active`、`inactive`。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callMediaState"
}-->
```json
{
  "audio": "active | inactive",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callMediaState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
