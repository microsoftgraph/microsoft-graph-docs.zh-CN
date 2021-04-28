---
title: oauth2permissiongrant： delta
description: 获取新创建、更新或删除的 oauth2permissiongrants，而无需执行整个资源集合的完整读取。
localization_priority: Normal
author: psignoret
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1317b50520d7e80e918141b9526e5691ceddf6ac
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055874"
---
# <a name="oauth2permissiongrant-delta"></a>oauth2permissiongrant： delta

命名空间：microsoft.graph

获取新创建、更新或删除的 [oauth2permissiongrant](../resources/oauth2permissiongrant.md) 对象，而无需执行整个资源集合的完整读取。 有关详细信息，请参阅使用 [delta 查询](/graph/delta-query-overview)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|oauth2permissiongrant | Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求


<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants/delta
```

## <a name="query-parameters"></a>查询参数

跟踪更改将引发一次或多组 **delta** 函数调用。 如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。 Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。 只需指定查询参数一次。 在后续请求中，复制并应用 `nextLink` 上 `deltaLink` 一响应中的 或 URL。 URL 包括编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 对[同一](/graph/delta-query-overview)资源集合之前的 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。  在集合的下一轮更改跟踪的第一个请求中保存和应用整个 `deltaLink` URL（包括此令牌）。|
| $skiptoken | string | 之前的[delta](/graph/delta-query-overview)函数调用的 URL 中返回的状态令牌，指示同一资源集合中还有进一步 `nextLink` 的更改需要跟踪。  |

### <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 OData 查询参数来帮助自定义响应。

- 查询参数 `$select` 可用于仅指定获得最佳性能所需的属性。 始终返回 **id** 属性。
- `$filter`查询参数只能用于通过使用资源 ID 跟踪特定资源的更改。 例如， `$filter=id+eq+{value}` `$filter=id+eq+{value1}+or+id+eq+{value2}` 或 。


## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [oauth2permissiongrant](../resources/oauth2permissiongrant.md) 集合对象。 该响应还包括 `nextLink`URL 或 `deltaLink`URL。

- 如果 `nextLink` 返回 URL，可以在会话中检索其他数据页。 **oauth2permissiongrant** 继续使用 URL 提出请求，直到 `nextLink` `deltaLink` 响应中包括 URL。
- 如果 `deltaLink` 返回 URL，则不返回有关资源的更多数据。 保留并使用 `deltaLink` URL 了解将来对资源的更改。

有关详细信息，请参阅使用 [delta 查询](/graph/delta-query-overview)。 有关示例请求，请参阅 [获取用户的增量更改](/graph/delta-query-users)。

## <a name="example"></a>示例
### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/oauth2permissiongrant-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/oauth2permissiongrant-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/oauth2permissiongrant-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/oauth2permissiongrant-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
      "id": "cMmjItSKIEGBJzAIN_h_LJWd3Ji2SVpAs8CDTpaacIs33-jCp8aITYmx_rTx_afF"
    }
  ]
}
```

<!-- uuid: ba679d55-d10e-4518-b733-6f3e9576afb1
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oauth2permissiongrant: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

