---
title: 创建 externalItem
description: 创建新的 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 170c3fb87903e6f2f66fe910d80ca8f4a6e87b50
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366793"
---
# <a name="create-externalitem"></a>创建 externalItem

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [externalItem](../resources/externalitem.md)。

此 API 可用于创建自定义项。 在 JSON 正文中包括 属性 `@odata.type` ，指定要创建的类型。 包含 [externalConnection](../resources/externalconnection.md) 的架构 [必须已](../resources/schema.md) 注册相应类型。

## <a name="permissions"></a>Permissions

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

| 参数     | 类型   | 说明                                         |
|:--------------|:-------|:----------------------------------------------------|
| connection-id | string | `id`包含[externalConnection 的 属性](../resources/externalconnection.md) |
| item-id       | string | 由开发人员提供的 `id` [externalItem 属性](../resources/externalitem.md)。 如果不存在此项目，将 `id` 创建一个新项。 如果项目已存在， `id` 则它将被正文中发送的对象覆盖。 |

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
|:--------------|:----------------------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [externalItem](../resources/externalitem.md) 对象的 JSON 表示形式。 有效负载限制为 4 MB。

### <a name="creating-an-externalitem"></a>创建 externalItem

创建 时 `externalItem` ，以下字段是必需的 `@odata.type` ：、和 `acl` `properties` 。 `properties`对象必须至少包含一个属性。

所有 `DateTime` 类型属性都必须采用 ISO 8601 格式。

在下列 `externalItem` 情况下，上的 属性应在有效负载中使用类型说明符：

- 对于 `String` 类型属性，如果值包含非 ASCII 字符。

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
    > 当包含 类型的 属性 `Collection(DateTime)` 时，必须使用类型说明器 `Collection(DateTimeOffset)` 。

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
PUT https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
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
