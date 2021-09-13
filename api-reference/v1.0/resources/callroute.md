---
title: callRoute 资源类型
description: 表示呼叫路由类型。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: be40f95a79802358bfa24fe57e94df895f3c4d2b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067505"
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

