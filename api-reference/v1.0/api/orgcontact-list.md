---
title: List orgContacts
description: 检索此组织的组织联系人列表。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 217ddcc7da6505db32596c233a987c4e99b7fb9c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207734"
---
# <a name="list-orgcontacts"></a>List orgContacts

命名空间：microsoft.graph

获取此组织的 [组织联系人](../resources/orgcontact.md) 列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 `$count`、`$expand`、`$filter`、`$orderBy`、`$search`、`$select` 和 `$top` [ OData 查询参数 ](/graph/query-parameters) 以帮助自定义响应。 只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:-----------|:----------|
| Authorization  |Bearer {token}。必需。 |
| ConsistencyLevel | 最终。 当使用 `$search` 或 `$filter` 的特定用法时，需要此标头和 `$count`。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [orgContact](../resources/orgcontact.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-get-organizational-contacts-for-an-organization"></a>示例 1：获取组织的组织联系人

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-orgcontact-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-orgcontact-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "companyName": "Contoso",
      "department": "Marketing",
      "displayName": "Eric S",
      "givenName":"Eric",
      "jobTitle":"Accountant",
      "mail":"erics@contoso.com",
      "mailNickname":"erics",
      "surname":"Solomon",
      "addresses":[
        {
          "city":"MyCity",
          "countryOrRegion":"United States",
          "officeLocation":"MyCity",
          "postalCode":"98000",
          "state":"WA",
          "street":"Contoso Way"
        }
      ],
      "phones":[
        {
          "number":"111-1111",
          "type":"businessFax"
        }
      ]
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a>示例 2：仅获取组织联系人的计数

#### <a name="request"></a>请求

下面展示了示例请求。 此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$count`。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

>**注意：**`$count`和`$search` 查询参数当前在 Azure AD B2C 租户中不可用。

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a>响应

下面介绍响应示例。

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a>示例 3：使用$filter和$top获取一个以“a”开头的显示名称（包括返回的对象计数）的组织联系人

#### <a name="request"></a>请求

下面展示了示例请求。 此请求需要将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串，因为请求同时具有 `$orderBy` 和 `$filter` 查询参数。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

>**注意：**`$count`和`$search` 查询参数当前在 Azure AD B2C 租户中不可用。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontacts_startswith"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontacts-startswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontacts-startswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontacts-startswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontacts-startswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-orgcontacts-startswith-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-orgcontacts-startswith-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.count":1,
  "value":[
    {
      "displayName":"Abigail Jackson",
      "mail":"abigailJ@contoso.com",
      "mailNickname":"abigailJ"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a>示例 4：使用$search获取包含字母“wa”的显示名称的组织联系人，其中包括返回的对象计数

#### <a name="request"></a>请求

下面展示了示例请求。 此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$search` 和 `$count=true` 查询字符串。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

>**注意：**`$count`和`$search` 查询参数当前在 Azure AD B2C 租户中不可用。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phone-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phone-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phone-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phone-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-phone-count-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-phone-count-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.count":22,
  "value":[
    {
      "displayName":"Nicole Wagner",
      "mail":"nicolewa@contoso.com",
      "mailNickname":"nicolewa"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

