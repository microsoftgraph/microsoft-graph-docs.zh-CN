---
title: 安全资源类型
description: 安全资源是安全对象模型的入口点。 它返回 singleton 安全资源。 它不包含任何可用的属性。
ms.openlocfilehash: ddf00e46135733ef18c18918c0c365134138671f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008558"
---
# <a name="security-resource-type"></a>安全资源类型

安全资源是安全对象模型的入口点。 它返回 singleton 安全资源。 它不包含任何可用的属性。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出警报](../api/alert-list.md) | [通知](alert.md)集合 | 获取通知对象集合。 |
| [获取通知](../api/alert-get.md) | [通知](alert.md)集合 | 获取通知对象。 |
| [更新通知](../api/alert-update.md) | [通知](alert.md)集合 | 获取通知对象。 |

## <a name="properties"></a>属性
无

## <a name="relationships"></a>Relationships
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|alerts|[通知](alert.md)集合| 只读。可为 NULL。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a>示例

可在图的根的**安全**资源。

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->