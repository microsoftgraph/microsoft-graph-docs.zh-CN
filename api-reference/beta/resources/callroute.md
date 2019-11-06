---
title: callRoute 资源类型
description: CallRoute 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 698cf2d6c2ae8b157aee4db45219eeb0b85c73c5
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006738"
---
# <a name="callroute-resource-type"></a>callRoute 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

CallRoute 类型。

## <a name="properties"></a>属性

| 属性            | 类型                          | 说明                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| 终稿               | [identitySet](identityset.md) | 在呼叫中解析为的标识。               |
| 源语言            | [identitySet](identityset.md) | 最初在呼叫中使用的标识。           |
| routingType         | String                        | 可取值为：`forwarded`、`lookup`、`selfFork`。  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
