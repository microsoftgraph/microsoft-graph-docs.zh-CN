---
title: callMediaState 资源类型
description: 表示呼叫的媒体状态。
author: ananmishr
ms.prod: cloud-communications
ms.localizationpriority: medium
doc_type: resourcePageType
ms.openlocfilehash: d07562bfaf14a69175535f8b38b73f56fdb0faa8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104360"
---
# <a name="callmediastate-resource-type"></a>callMediaState 资源类型

命名空间：microsoft.graph


表示呼叫的媒体 [状态](call.md)。

## <a name="properties"></a>属性

| 属性            | 类型    | 说明                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| audio           | mediaState  | 音频媒体状态。 可取值为：`active`、`inactive`、`unknownFutureValue`。 |

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

