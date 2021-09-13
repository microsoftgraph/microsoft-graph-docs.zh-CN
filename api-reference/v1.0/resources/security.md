---
title: 安全资源类型
description: 安全资源是安全对象模型的入口点。 它返回单一安全资源。 它不包含任何可用属性。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 14c0aa4a239b143df79d873e127c3e70dc7900fe
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139602"
---
# <a name="security-resource-type"></a>安全资源类型

命名空间：microsoft.graph

安全资源是安全对象模型的入口点。 它返回单一安全资源。 它不包含任何可用属性。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出警报](../api/alert-list.md) | [警报](alert.md)集合 | 获取 alert 对象集合。 |
| [获取警报](../api/alert-get.md) | [警报](alert.md)集合 | 获取警报对象。 |
| [更新警报](../api/alert-update.md) | [警报](alert.md)集合 | 获取警报对象。 |

## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|警报|[警报](alert.md)集合| 只读。可为空。|


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

**安全** 资源位于图形的根目录。

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
```http
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

