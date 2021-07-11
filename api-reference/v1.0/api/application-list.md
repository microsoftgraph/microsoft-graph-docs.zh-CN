---
title: 列出应用程序
description: 获取该组织中应用程序的列表。
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ede0058fd04db947d65da16f806321221be08f50
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350948"
---
# <a name="list-applications"></a>列出应用程序

命名空间：microsoft.graph

获取该组织中[应用程序](../resources/application.md)的列表。

> [!NOTE]
> 使用为个人 Microsoft 帐户颁发的令牌调用此 API 时，将返回个人 Microsoft 帐户所拥有的应用。 个人 Microsoft 帐户不存在组织概念。 为了列出特定个人 Microsoft 帐户所拥有的应用程序，此 API 需要用户。除 Application.Read.All 或 Application.ReadWrite.All 之外，还读取权限。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.Read.All、 Application.ReadWrite.All、 Directory.Read.All、 Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | Application.Read.All 和 User.Read， Application.ReadWrite.All 和 User.Read |
|应用程序 | Application.Read.All、Application.ReadWrite.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter` 可使用“**displayName**”和“**说明**”属性上的`$search`。 为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。 在添加或更新项目与在索引中可用之间可能会稍有延迟。

## <a name="request-headers"></a>请求标头

| 名称           | 说明                |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}。必需。  |
| ConsistencyLevel | 最终。 当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。 它使用的索引可能与对象的最新更改不同步。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-get-the-list-of-applications"></a>示例 1：获取应用程序列表

#### <a name="request"></a>请求

下面是一个请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面是一个响应示例。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications",
  "value": [
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName": "My app",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-applications"></a>示例 2：仅获取应用程序计数

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a>示例 3：使用 $filter 和 $top 获取一个显示名称以“a”开头的应用程序，其中包括返回的对象数

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
  "@odata.count":1,
  "value":[
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName":"a",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a>示例 4：使用 $search 获取显示名称中包含字母“Web”的应用程序，其中包括返回的对象数

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "ignored",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
  "@odata.count":1396,
  "value":[
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName":"'DotNetWeb-App' ",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
