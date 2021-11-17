---
title: orgContact： delta
description: 获取新建、更新或删除的组织联系人，而无需执行整个集合的完全读取。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9a736ac1320746a2e0e42ead7f546b13324b8bc7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018437"
---
# <a name="orgcontact-delta"></a>orgContact： delta

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取新建、更新或删除的组织联系人，而无需执行整个集合的完全读取。 有关详细信息，请参阅[更改跟踪](/graph/delta-query-overview)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。  |
|应用程序 | OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

若要开始跟踪更改，请对 contacts 资源提出包含 delta 函数的请求。

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/delta
```

## <a name="query-parameters"></a>查询参数

跟踪组织联系人的更改将引发一组 delta 函数调用。  如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。 Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。

只需指定任何查询参数一次。

在后续请求中，复制并应用 `nextLink` 上 `deltaLink` 一响应中的 或 URL。 该 URL 已包含编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 对[同](/graph/delta-query-overview)一组织联系人集合之前的 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。  在集合的下一轮更改跟踪的第一个请求中保存和应用整个 `deltaLink` URL（包括此令牌）。|
| $skiptoken | string | 之前的[delta](/graph/delta-query-overview)函数调用的 URL 中返回的状态令牌，指示同一组织联系人集合中还有进一步 `nextLink` 的更改需要跟踪。  |

### <a name="odata-query-parameters"></a>OData 查询参数

此方法支持可选的 OData 查询参数来帮助自定义响应。

- 像在任何 GET 请求中一样，您可以使用查询参数来仅指定 `$select` 获得最佳性能所需的属性。 始终返回 **id** 属性。
- 提供对 `$filter` 的有限支持：
  - 唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。 可以筛选多个对象。 例如，`https://graph.microsoft.com/beta/contacts/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。 筛选对象不能超出 50 个。

## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者 &lt;token&gt;。必需。|
| Prefer | return=minimal <br><br>在使用 `deltaLink` 的请求中执行此标头将仅返回自上一轮之后发生更改的对象属性。 可选。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [orgContact](../resources/orgcontact.md) 集合对象。 该响应还包括 `nextLink`URL 或 `deltaLink`URL。

- 如果返回 `nextLink`URL：
  - 这表示绘画中存在要检索的其他数据页面。 应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。
  - 响应包含与初始 Delta 查询请求相同的属性集。 这使你能够在发起 Delta 循环时捕获对象当前的完整状态。

- 如果返回 `deltaLink`URL：
  - 这表示不再返回有关资源现有状态的数据。 保存并使用 `deltaLink` URL 来了解下一轮资源更改。
  - 只有对于在签发 `deltaLink` 之后更改的属性，你才可以选择指定 `Prefer:return=minimal` 标头以包含在响应值中。

### <a name="default-return-the-same-properties-as-initial-delta-request"></a>默认：返回与初始 Delta 请求相同的属性

默认情况下，使用 `deltaLink` 或 `nextLink` 的请求将通过以下方式返回与初始 Delta 查询中选择的相同属性：

- 如果属性已更改，则新值将包括在响应中。 这包括设为 Null 值的属性。
- 如果属性未更改，则旧值将包括在响应中。
- 如果之前从未设置过该属性，则它完全不会包含在响应中。


> **注意：** 通过此行为，无法通过查看响应来判断属性是否正在更改。 此外，增量响应往往很大，因为它们包含所有属性值，如示例 [2 所示](#example-2-selecting-three-properties)。

### <a name="alternative-return-only-the-changed-properties"></a>备用：仅返回更改的属性

添加可选请求标头 - `prefer:return=minimal` - 将导致出现以下行为：

- 如果属性已更改，则新值将包括在响应中。 这包括设为 Null 值的属性。
- 如果尚未更改属性，则该属性不会包括在响应中。（不同于默认行为。）

> **注意：** 可以在 Delta 循环中的任何时间点将标头添加到 `deltaLink` 请求中。 标头仅影响响应中包含的属性集，而不会影响增量查询的运行。 请参阅[示例 3](#example-3-alternative-minimal-response-behavior)。

## <a name="examples"></a>示例

### <a name="example-1-default-properties"></a>示例 1：默认属性

#### <a name="request"></a>请求

下面展示了示例请求。 因为没有参数 `$select` ，因此将跟踪并返回一组默认属性。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgContact_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/orgcontact-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/beta/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "id": "string (identifier)",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mailNickname": "mailNickname-value",
      "surname": "surname-value"
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
  "name": "orgcontact_delta_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/delta?$select=displayName,jobTitle,mail
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/orgcontact-delta-select-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。 请注意，所有三种属性将包括在响应中，并且无法知道在获得 `deltaLink` 之后哪些属性发生了更改。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/beta/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mail": null
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
  "name": "orgcontact_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/delta?$select=displayName,jobTitle,mail
Prefer: return=minimal
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/orgcontact-delta-minimal-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。 请注意，不包括属性，这意味着它自上次 delta 查询以来没有更改;和 包含在内， `mail` `displayName` `jobTitle` 这意味着其值已更改。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/beta/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```
## <a name="see-also"></a>另请参阅

- [使用 Delta 查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)。

<!-- uuid: 3B5A9A7C-6324-432F-8C66-AC4883DD71EF
2020-03-20 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


