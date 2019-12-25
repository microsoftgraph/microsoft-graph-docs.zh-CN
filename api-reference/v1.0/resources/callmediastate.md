---
title: callMediaState 资源类型
description: 表示呼叫的媒体状态。
author: VinodRavichandran
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 01e2e8017d89ddf96997d1d5bef729f9e9dc439d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871082"
---
# <a name="callmediastate-resource-type"></a>callMediaState 资源类型


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
