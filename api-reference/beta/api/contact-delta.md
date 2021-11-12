---
title: 'contact: delta'
description: 获取指定文件夹中已添加、删除或更新的联系人集。
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8d57707ef63363f3acf4ac1b9ebf40b35d8527e4
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60942399"
---
# <a name="contact-delta"></a>contact: delta

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取指定文件夹中已添加、删除或更新的联系人集。

对文件夹中的联系人的 **delta** 函数调用与 GET 请求相似，但是可通过在对其的一次或多次调用中正确应用 [状态令牌](/graph/delta-query-overview)来查询该文件夹中的联系人的增量更改这一点除外。通过此功能，你可以维护和同步本地存储的用户联系人，而无需每次都从服务器中获取整组联系人。  

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Contacts.Read、Contacts.ReadWrite    |
|委派（个人 Microsoft 帐户） | Contacts.Read、Contacts.ReadWrite    |
|应用程序 | Contacts.Read、Contacts.ReadWrite |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/contacts/delta
GET /users/{id}/contactFolders/{id}/contacts/delta
```

## <a name="query-parameters"></a>查询参数

跟踪联系人更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 对同一个联系人集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 之前的 **delta** 函数调用的 `nextLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示同一个联系人集合中有进一步的更改需要跟踪。 |

### <a name="odata-query-parameters"></a>OData 查询参数

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。 


## <a name="request-headers"></a>请求头
| 名称       | 类型 | 说明 |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type  | string  | application/json. Required. |
| Prefer | string  | odata.maxpagesize={x}。可选。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contact](../resources/contact.md) 集合对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面的示例演示了如何调用单个 **delta** 函数，使用 `$select` 参数仅获取每个联系人的 **displayName** 属性并将响应正文中的联系人的最大数目限制为 2。

若要跟踪文件夹中联系人的更改，要使用正确的状态令牌执行一次或多次 **delta** 函数调用来获取上次增量查询后的增量更改集。 

演示如何使用状态令牌跟踪邮件文件夹中的邮件更改的示例与其相似：[获取文件夹中邮件的增量更改](/graph/delta-query-messages)。跟踪联系人和跟踪文件夹中的邮件之间的主要区别在于增量查询请求 URL 以及查询响应将返回 **mailFolder** 集合而非 **message** 集合。
 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts/delta?$select=displayName

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contact-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
如果请求成功，响应将包含一个状态令牌，其为 _skipToken_  
（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。

以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。

注意：为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/contactfolders/{id}/contacts/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

### <a name="see-also"></a>另请参阅

- [Microsoft Graph 增量查询](/graph/delta-query-overview)
- [获取文件夹中邮件的增量更改](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
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


