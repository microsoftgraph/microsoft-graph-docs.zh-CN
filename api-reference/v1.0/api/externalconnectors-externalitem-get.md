---
title: 获取 externalItem
description: 读取 externalItem 对象的属性和关系。
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 1c36751b9463454f1251cc7ca269054791ca9ed5
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133459"
---
# <a name="get-externalitem"></a>获取 externalItem
命名空间：microsoft.graph.externalConnectors



读取 [externalItem](../resources/externalconnectors-externalitem.md) 对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
| 委派（工作或学校帐户）     | ExternalItem.ReadWrite.OwnedBy、ExternalItem.Read.All、ExternalItem.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持                               |
| 应用程序                            | ExternalItem.ReadWrite.OwnedBy、ExternalItem.Read.All、ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /external/connections/{connectionsId}/items/{externalItemId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法不支持自定义响应的可选查询参数。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [externalItem](../resources/externalconnectors-externalitem.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
下面展示了示例请求。

```http
GET https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
```


### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant"
    },
    {
      "type": "externalGroup",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "Error in payment gateway...",
    "type": "text"
  }
}
```

