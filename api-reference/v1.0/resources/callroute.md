---
title: callRoute 资源类型
description: 表示呼叫路由类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 82d69edb17d1a68ab3fc0f22402bd26c94c02dd3f922f0eb091cce95ce0b921f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141817"
---
# <a name="callroute-resource-type"></a>callRoute 资源类型

命名空间：microsoft.graph

表示呼叫路由类型。

## <a name="properties"></a>属性

| 属性            | 类型                          | 说明                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| final               | [identitySet](identityset.md) | 在呼叫中解析到的标识。               |
| 源语言            | [identitySet](identityset.md) | 最初在调用中使用的标识。           |
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

