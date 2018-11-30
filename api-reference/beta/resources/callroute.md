---
title: callRoute 资源类型
description: CallRoute 类型。
ms.openlocfilehash: d2a85d34fe755c6e725abc9a1308a3837f0acf3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043705"
---
# <a name="callroute-resource-type"></a>callRoute 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

CallRoute 类型。

## <a name="properties"></a>属性

| 属性            | 类型                          | 说明                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| 最终               | [identitySet](identityset.md) | 解析为呼叫中的标识。               |
| 源语言            | [identitySet](identityset.md) | 最初在呼叫中使用的标识。           |
| routingType         | 字符串                        | 可取值为：`forwarded`、`lookup`、`selfFork`。  |

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
<!-- {
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
