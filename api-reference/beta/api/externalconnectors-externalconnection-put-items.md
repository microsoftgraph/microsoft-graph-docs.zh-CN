---
title: 创建 externalItem
description: 创建新的 externalItem。
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 49cf69b49edda6c8a7ea7a97d2ef826ce1bd5bce
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133438"
---
# <a name="create-externalitem"></a>创建 externalItem

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [externalItem](../resources/externalconnectors-externalitem.md)。

此 API 可用于创建自定义项。 包含 [的 externalConnection](../resources/externalconnectors-externalconnection.md) 必须注册相应类型的 [架构](../resources/externalconnectors-schema.md) 。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>路径参数

| 参数     | 类型   | 说明                                         |
|:--------------|:-------|:----------------------------------------------------|
| connection-id | string | `id`包含 [externalConnection](../resources/externalconnectors-externalconnection.md) 的属性 |
| item-id       | string | [externalItem](../resources/externalconnectors-externalitem.md) 的开发人员提供的`id`属性。 如果此 `id`项中尚不存在任何项，则会创建一个新项。 如果此项已存在 `id`，则由在正文中发送的对象覆盖该项。 |

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
|:--------------|:----------------------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [externalItem](../resources/externalconnectors-externalitem.md) 对象的 JSON 表示形式。 有效负载限制为 4 MB。

### <a name="creating-an-externalitem"></a>创建 externalItem

创建某个`externalItem`字段时，需要以下字段： `acl``properties` 该 `properties` 对象必须至少包含一个属性。

所有 `DateTime` 类型属性都必须采用 ISO 8601 格式。

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

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections",
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
}-->

```http
PUT https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    },
    {
      "type": "group",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny",
      "identitySource": "external"
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
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-externalitem-from-connections-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>响应
<!-- markdownlint-enable MD024 -->

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
