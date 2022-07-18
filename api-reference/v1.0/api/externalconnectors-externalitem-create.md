---
title: 创建 externalItem
description: 创建新的 externalItem。
author: snlraju-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6c670eb174b410519de41d78f8c2fdab694566a2
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133029"
---
# <a name="create-externalitem"></a>创建 externalItem

命名空间：microsoft.graph.externalConnectors

创建新的 [externalItem](../resources/externalconnectors-externalitem.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
| 委派（工作或学校帐户）     | ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持                               |
| 应用程序                            | ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [externalItem](../resources/externalconnectors-externalitem.md) 对象的 JSON 表示形式。

创建 [externalItem](../resources/externalconnectors-externalitem.md) 时，可以指定以下属性。

|属性|类型| 说明|
|:---|:---|:---|
|id|String|项 ID。 必需。|
|properties|[microsoft.graph.externalConnectors.properties](../resources/externalconnectors-properties.md)|项属性。 该 `properties` 对象必须至少包含一个属性。 所有 `DateTime` 类型属性都必须采用 ISO 8601 格式。 必需。|
|content|[microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md)|外部项内容。 可选。|
|Acl|[microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) 集合|访问控制列表。 必需。|

在以下方案中，某个属性 `externalItem` 应在有效负载中使用类型说明符：

- 对于 `String` 类型属性，如果该值包含非 ASCII 字符。

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- 对于所有集合类型。

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > 包括类型的 `Collection(DateTime)`属性时，必须使用类型说明符 `Collection(DateTimeOffset)`。

## <a name="response"></a>响应 

如果成功，此方法返回 `200 OK` 响应代码。

## <a name="examples"></a>示例

### <a name="example-create-a-custom-item"></a>示例：创建自定义项

### <a name="request"></a>请求



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_externalConnections"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/external/connections/contosohr/items/TSP228082938
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-externalconnections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-externalconnections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-externalconnections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-externalitem-from-externalconnections-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

