---
title: 'user: delta'
description: 获得新建、更新或删除的用户，无需对整个用户集合执行完整读取。
ms.localizationpriority: high
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 46a1c1c89d96a6117e5dddfbb6e1c42f30157b59
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247355"
---
# <a name="user-delta"></a>user: delta

命名空间：microsoft.graph

获取新建、更新或删除的用户，无需对整个用户集合执行完整读取。有关详细信息，请参阅[更改跟踪](/graph/delta-query-overview)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

为开始跟踪更改，请在用户资源上发出包含 delta 函数的请求。

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a>查询参数

跟踪用户的更改会触发一个或多个 **delta** 函数调用。如果使用任何查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在初始 **delta** 请求中指定它。Microsoft Graph 会自动将任何指定参数编码为响应中返回的 `@odata.nextLink` 或 `@odata.deltaLink` URL 的令牌部分。

只需预先指定所需的任何查询参数一次。

在后续请求中，可以复制并应用之前响应中返回的 `@odata.nextLink` 或 `@odata.deltaLink` URL，因为此 URL 已包含所需的编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 对同一个用户集合之前的 **delta** 函数调用的 `@odata.deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `@odata.deltaLink` URL。|
| $skiptoken | string | 对之前的 **delta** 函数调用的 `@odata.nextLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示同一个用户集合中有进一步的更改需要追踪。 |

### <a name="odata-query-parameters"></a>OData 查询参数

此方法支持可选 OData 查询参数来帮助自定义响应。

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。
- 提供对 `$filter` 的有限支持：
  - 唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。 可以筛选多个对象。 例如，`https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。 筛选对象不能超出 50 个。

## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者&lt;令牌&gt;|
| Content-Type  | application/json |
| Prefer | return=minimal <br><br>在使用 `@odata.deltaLink` 的请求中执行此标头将仅返回自上一轮之后发生更改的对象属性。可选。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法的响应正文将返回`200 OK`响应代码和[用户](../resources/user.md)集合对象。响应还包括 `@odata.nextLink` URL 或 `@odata.deltaLink` URL。

- 如果返回 `@odata.nextLink`URL：
  - 这表明会话中存在要检索的其他数据页面。应用程序继续使用 `@odata.nextLink` URL 发出请求，直到响应中包含 `@odata.deltaLink` URL。
  - 响应包含与初始 Delta 查询请求相同的属性集。 这使你能够在发起 Delta 循环时捕获对象当前的完整状态。

- 如果返回 `@odata.deltaLink`URL：
  - 这表示未返回关于资源现有状态的更多数据。 保存并使用 `@odata.deltaLink` URL 来了解下一轮资源更改。
  - 只有对于在签发 `@odata.deltaLink` 之后更改的属性，你才可以选择指定 `Prefer:return=minimal` 标头以包含在响应值中。

### <a name="default-return-the-same-properties-as-initial-delta-request"></a>默认：返回与初始 Delta 请求相同的属性

默认情况下，使用 `@odata.deltaLink` 或 `@odata.nextLink` 的请求将通过以下方式返回与初始 Delta 查询中选择的相同属性：

- 如果属性已更改，则新值将包括在响应中。 这包括设为 Null 值的属性。
- 如果属性未更改，则旧值将包括在响应中。
- 如果之前从未设置属性，则它不会包括在响应中。


> **注意：** 如果出现此行为，那么通过查看响应无法区分属性是否已更改。 此外，Delta 响应往往过大，因为它们包含所有属性值，如[示例 2](#example-2-selecting-three-properties) 所示。

### <a name="alternative-return-only-the-changed-properties"></a>备用：仅返回更改的属性

添加可选请求标头 - `prefer:return=minimal` - 将导致出现以下行为：

- 如果属性已更改，则新值将包括在响应中。 这包括设为 Null 值的属性。
- 如果尚未更改属性，则该属性不会包括在响应中。（不同于默认行为。）

> **注意：** 可以在 Delta 循环中的任何时间点将标头添加到 `@odata.deltaLink` 请求中。 标头仅影响响应中包含的属性集，它不会影响执行 Delta 查询的方式。 请参阅[示例 3](#example-3-alternative-minimal-response-behavior)。

## <a name="examples"></a>示例

### <a name="example-1-default-properties"></a>示例 1：默认属性

#### <a name="request"></a>请求

下面展示了示例请求。 没有 `$select` 参数，因为将跟踪并返回默认的属性集。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

以下示例所示为使用从查询初始化获得的 `@odata.deltaLink` 时的响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "+1 425 555 0109"
      ],
      "displayName": "Adele Vance",
      "givenName": "Adele",
      "jobTitle": "Retail Manager",
      "mail": "AdeleV@contoso.onmicrosoft.com",
      "mobilePhone": "+1 425 555 0109",
      "officeLocation": "18/2111",
      "preferredLanguage": "en-US",
      "surname": "Vance",
      "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
      "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
    }
  ]
}
```
### <a name="example-2-selecting-three-properties"></a>示例 2：选择三个属性

#### <a name="request"></a>请求

下一个示例所示为通过默认响应行为选择三种更改跟踪属性时的初始请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-delta-select-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-delta-select-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

以下示例所示为使用从查询初始化获得的 `@odata.deltaLink` 时的响应。 请注意，所有三种属性将包括在响应中，并且无法知道在获得 `@odata.deltaLink` 之后哪些属性发生了更改。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "Adele Vance",
      "jobTitle": "Retail Manager",
      "mobilePhone": "+1 425 555 0109"
    }
  ]
}
```

### <a name="example-3-alternative-minimal-response-behavior"></a>示例 3：备用最小响应行为

#### <a name="request"></a>请求

下一个示例所示为通过备用最小响应行为选择三种更改跟踪属性时的初始请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-delta-minimal-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-delta-minimal-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

以下示例所示为使用从查询初始化获得的 `@odata.deltaLink` 时的响应。 请注意，`mobilePhone` 属性不包括在内，这意味着它在上一轮 Delta 查询之后未发生更改；并且 `displayName` 和 `jobTitle` 将包括在内，这意味着其值已发生更改。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "Vance Adele",
      "jobTitle": "Product Marketing Manager"
    }
  ]
}
```
## <a name="see-also"></a>另请参阅

- [使用 Delta 查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)。
- [获取用户的增量更改](/graph/delta-query-users)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

