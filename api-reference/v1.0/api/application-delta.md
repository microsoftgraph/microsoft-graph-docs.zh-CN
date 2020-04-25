---
title: 应用程序： delta
description: 获取已创建、更新或删除的应用程序，而不执行整个资源集合的完全读取。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 88e49e674a3dd19cf8a97d2a6cbf5c989fd4f63c
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806662"
---
# <a name="application-delta"></a>应用程序： delta

命名空间：microsoft.graph

获得新建、更新或删除的应用，无需完全读取整个资源集合。 有关详细信息，请参阅[Using delta query](/graph/delta-query-overview)。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.ReadWrite.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 请求

若要开始跟踪更改，请在**应用程序**资源上发出包含 delta 函数的请求。 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

## <a name="query-parameters"></a>查询参数

跟踪更改会产生一个或多个**delta**函数调用的往返。 如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。 Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。 您只需提前指定任何查询参数。 在后续请求中，复制并应用`nextLink`上`deltaLink`一个响应中的或 URL。 该 URL 已包含已编码的参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 为同一资源集合在上`deltaLink`一个**delta**函数调用的 URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该往返一轮的更改。 将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 在上一个**delta**函数调用`nextLink`的 URL 中返回的[状态令牌](/graph/delta-query-overview)，指示在同一资源集合中有进一步的更改需要跟踪。 |

### <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 OData 查询参数来帮助自定义响应。

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 **id** 属性。
- 提供对 `$filter` 的有限支持：
  * 唯一受支持`$filter`的表达式是跟踪对特定资源所做的更改，其`$filter=id+eq+{value}` ID `$filter=id+eq+{value1}+or+id+eq+{value2}`：或。 您可以指定的 Id 数受最大 URL 长度的限制。


## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者 &lt;token&gt;。 必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和[application](../resources/application.md)集合对象。 该响应还包括 `nextLink`URL 或 `deltaLink`URL。

- 如果返回`nextLink` URL，则会在会话中检索其他数据页。 应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。
- 如果返回`deltaLink` URL，则没有有关要返回的资源的现有状态的更多数据。 保留并使用`deltaLink` URL 了解将来对资源所做的更改。

有关详细信息，请参阅[Using delta query](/graph/delta-query-overview)。 有关示例请求，请参阅[获取用户的增量更改](/graph/delta-query-users)。

## <a name="example"></a>示例
### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
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
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
