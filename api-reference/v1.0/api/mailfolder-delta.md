---
title: 'mailFolder: delta'
description: 获取用户邮箱中已添加、删除或移除的邮件文件夹集。
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2066d7398690a3bef39a25ec3cdf31de4372dbfe
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60924528"
---
# <a name="mailfolder-delta"></a>mailFolder: delta

命名空间：microsoft.graph

获取用户邮箱中已添加、删除或移除的邮件文件夹集。

对邮箱的邮件文件夹的 **delta** 函数调用与 GET 请求相似，除了前者可通过在对其的一次或多次调用中正确应用 [状态令牌](/graph/delta-query-overview)来查询邮件文件夹中的增量更改。通过此功能，你可以维护和同步本地存储的用户邮件文件夹，而无需每次都从服务器中获取该邮箱的所有邮件文件夹。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Mail.ReadBasic、Mail.Read、Mail.ReadWrite    |
|委派（个人 Microsoft 帐户） | Mail.ReadBasic、Mail.Read、Mail.ReadWrite    |
|应用程序 | Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/delta
GET /users/{id}/mailFolders/delta
```

## <a name="query-parameters"></a>查询参数

跟踪邮件文件夹更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 对同一个邮件文件夹集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，其指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 对之前的 **delta** 函数调用的 `nextLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示同一个邮件文件夹集合中有进一步的更改需要追踪。 |

### <a name="odata-query-parameters"></a>OData 查询参数

像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。 

## <a name="request-headers"></a>请求头
| 名称       | 类型 | 说明 |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type  | string  | application/json. Required. |
| Prefer | string  | odata.maxpagesize={x}。可选。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 集合对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
以下示例演示了如何执行单次 **delta** 函数调用，并将响应正文中的邮件文件夹最大数目限制为 2。

若要跟踪邮箱的邮件文件夹的更改，要使用正确的状态令牌执行一次或多次 **delta** 函数调用来获取上一次增量查询后的增量更改集。 

你可以找到一个类似的示例，演示如何使用状态令牌跟踪邮件文件夹中的邮件更改：[获取文件夹中邮件的增量更改](/graph/delta-query-messages)。跟踪邮件文件夹和跟踪文件夹中的邮件之间的主要区别在于，增量查询请求 URL 以及查询响应将返回 **mailFolder** 集合而非 **message** 集合。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/delta

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-delta-java-snippets.md)]
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
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99
    }
  ]
}
```

### <a name="see-also"></a>另请参阅

- [使用增量查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)
- [获取文件夹中邮件的增量更改](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

