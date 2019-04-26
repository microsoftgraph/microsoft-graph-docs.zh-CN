---
title: callRoute 资源类型
description: callRoute 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 06dd1a2265c5a6bda9feba0b51e7fd731d7945c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328274"
---
# <a name="callroute-resource-type"></a>callRoute 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

callRoute 类型。

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
