---
title: 创建 externalItem
description: 创建新的 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6e0ee2ca2eebcca9b912c62242c2606590d9cbc4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192264"
---
# <a name="create-externalitem"></a>创建 externalItem

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [externalItem](../resources/externalitem.md)。

此 API 可用于创建自定义项。 通过在 JSON 正文中包含属性来指定要创建的类型 `@odata.type` 。 包含的 [externalConnection](../resources/externalconnection.md) 必须具有相应类型的已注册 [架构](../resources/schema.md) 。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>路径参数

| 参数     | 类型   | 描述                                         |
|:--------------|:-------|:----------------------------------------------------|
| connection-id | string | `id`包含[externalConnection](../resources/externalconnection.md)的属性 |
| item-id       | string | ExternalItem 的开发人员提供的 `id` 属性[externalItem](../resources/externalitem.md)。 如果不存在具有此项的项目 `id` ，则会创建一个新项目。 如果某个项目已经存在，则 `id` 会被在正文中发送的对象覆盖。 |

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
|:--------------|:----------------------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [externalItem](../resources/externalitem.md) 对象的 JSON 表示形式。 有效负载限制为 4 MB。

### <a name="creating-an-externalitem"></a>创建 externalItem

在创建时 `externalItem` ，需要以下字段： `@odata.type` 、 `acl` 和 `properties` 。 该 `properties` 对象必须至少包含一个属性。

所有 `DateTime` 类型属性都必须采用 ISO 8601 格式。

中的属性 `externalItem` 应在以下方案中使用有效负载中的类型说明符：

- 对于 `String` type 属性，如果该值包含非 ASCII 字符。

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- 适用于所有集合类型。

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > 如果包含类型的属性 `Collection(DateTime)` ，则必须使用类型说明符 `Collection(DateTimeOffset)` 。

## <a name="response"></a>响应

如果成功，此方法返回 `200 OK` 响应代码。

## <a name="examples"></a>示例

### <a name="example-create-a-custom-item"></a>示例：创建自定义项

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
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
